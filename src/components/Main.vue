<template>
  <main>
    <div class="btn">
      current series
    </div>
    <div class="main-wrapper">
      <ProductCard
        v-for="(singleCard, index) in cards"
        :key="index"
        :card="singleCard"
      />
    </div>

    <div class="btn-load">
    <a href="#">
      load more
    </a>
    </div>
  </main>
</template>

<script>
import cards from "../assets/data/dc-comics";
import ProductCard from "./ProductCard.vue";

export default {
  components: { ProductCard },
  name: "Main",
  data() {
    return {
      cards,
    };
  },
  mounted() {
    console.log(cards);
  },
};
</script>

<style lang="scss" scoped>
// importo le variabili
@import "../assets/style/vars.scss";
main {
  position: relative;
  padding: 40px 210px;
  .btn {
    position: absolute;
    top: -23px;
    padding: 10px;
    text-align: center;
    text-transform: uppercase;
    color: white;
    background-color: $brand-color;
    border: 1px solid $brand-color;
    font-size: 1.2em;
    z-index: 1;
  }
  .main-wrapper {
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
  }
  .btn-load {
    width: 250px;
    padding: 10px;
    margin: 0 auto;
    margin-top: 40px;
    text-align: center;
    text-transform: uppercase;
    background-color: $brand-color;
    border: 1px solid $brand-color;
    cursor: pointer;
    &:hover {
      filter: brightness(1.2);
    }
    a {
      color: white;
    }
  }
}
</style>
