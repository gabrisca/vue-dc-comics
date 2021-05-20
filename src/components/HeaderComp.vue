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
          v-for="(link, index) in links" :key="index"
        >
          <a 
          :class="{'active': link.current}"
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
          url: '#',
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
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
  // importo le variabili
  @import '../assets/style/vars.scss';
  header {
    height: 100px;
    background-color: #FFFFFF;
    margin-top: 40px;
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
          li {
            margin-left: 25px;
              a {
                color: #484D52;
                text-decoration: none;
                text-transform: uppercase;
                &:hover {
                  color: $brand-color;
                }
                &.active {
                  padding-bottom: 36px;
                  border-bottom: 4px solid $brand-color;
                }
              }
          }
        }
      }
  }
</style>