<template>
  <div id="strip">
    
      <div class="wrapper">
        <div
          class="commercial"
          v-for="(commercial, index) in commercials"
          :key="index"
        >
          <a href="#">
            <img :src="commercial.image" :alt="commercial.text" />
            <span>
              {{ commercial.text }}
            </span>
          </a>
        </div>
      </div>
   
  </div>
</template>

<script>
export default {
  name: "BlueBand",
  data() {
    return {
      commercials: [
        {
          image: require("../assets/img/buy-comics-digital-comics.png"),
          text: "digital comics",
        },
        {
          image: require("../assets/img/buy-comics-merchandise.png"),
          text: "dc merchandise",
        },
        {
          image: require("../assets/img/buy-comics-subscriptions.png"),
          text: "subscription",
        },
        {
          image: require("../assets/img/buy-comics-shop-locator.png"),
          text: "comic shop locator",
        },
        {
          image: require("../assets/img/buy-dc-power-visa.svg"),
          text: "dc power visa",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
#strip {

  padding: 40px 230px;
  background-color: #0c82f9;
    .wrapper {
        display: flex;
      .commercial {
        flex-basis: calc(100% / 5);
        a {
          display: flex;
          align-items: center;
          color: white;
          img {
            height: 50px;
            margin-right: 5px;
          }
          span {
            text-transform: uppercase;
            font-size: 0.8em;
          }
        }
      }
    }
  
}
</style>
