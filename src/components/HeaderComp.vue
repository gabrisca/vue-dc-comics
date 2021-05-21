<template>
  <header class="container">
    <div id="logo">
      <a href="#">
        <img src="../assets/img/dc-logo.png" alt="logo DC Comics">
      </a>
    </div>
    <div id="menu">
      <ul>
        <li  
          v-for="(link, index) in links" 
          :key="index"
          @click.stop="setActive(index)"
          :class="{'active': link.current}"
        >
          <a 
          :href="link.url"
          >
          {{link.text}}
          </a>
        </li>
      </ul>
    </div>
  </header>
</template>

<script>
export default {
  name: 'HeaderComp',
  data(){
    return {
      links: [
        {
          text: 'caracters',
          url: 'javascript:void(0)',
          current: false
        },
        {
          text: 'comics',
          url: '#',
          current: true
        },
        {
          text: 'movies',
          url: '#',
          current: false
        },
        {
          text: 'tv',
          url: '#',
          current: false
        },
        {
          text: 'games',
          url: '#',
          current: false
        },
        {
          text: 'collectibles',
          url: '#',
          current: false
        },
        {
          text: 'videos',
          url: '#',
          current: false
        },
        {
          text: 'fans',
          url: '#',
          current: false
        },
        {
          text: 'news',
          url: '#',
          current: false
        },
        {
          text: 'shop',
          url: '#',
          current: false
        },
      ],
    }
  },
  mounted(){

  },
  methods: {
    // function active al click
    setActive(index) {
      this.links.forEach((link) => {
        link.current = false
      })
      this.links[index].current = true
    }
  },
}
</script>

<style lang="scss" scoped>
  // importo le variabili
  @import '../assets/style/vars.scss';
  header {
    height: 100px;
    background-color: #FFFFFF;
    display: flex;
    justify-content: space-between;
    align-items: center;
      #logo {
        margin: 10px 0;
        height: 80px;
          a {
            img {
              height: 100%;
            }
          }
      }
      #menu {
        ul {
          display: flex;
          align-items: center;
          flex-wrap: wrap;
          li {
            margin-left: 25px;
            height: 100px;
            line-height: 100px;
            cursor: pointer;
            &.active {
                  border-bottom: 4px solid $brand-color;
                  a {
                    color: $brand-color;
                  }
                }
            &:hover a{
                  color: $brand-color;
                }
              a {
                color: #484D52;
                height: 100%;
                text-decoration: none;
                text-transform: uppercase;
              }
          }
        }
      }
  }
</style>