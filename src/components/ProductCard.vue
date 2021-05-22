<template>
  <div id="album">
    <img :src="card.thumb" :alt="card.series">
    <span>{{card.series}}</span>
  </div>
</template>

<script>
export default {
  name: 'ProductCard',
  props: {
    card: Object
  }
}
</script>

<style lang="scss" scoped>
  #album {
    flex-basis: calc(100% / 6);
    margin-bottom: 20px;
    cursor: pointer;
    margin: 10px;
    &:hover {
      filter: brightness(1.2);
    }
    img {
      margin-bottom: 10px;
    }
    span {
      display: block;
      color: white;
      text-transform: uppercase;
    }
  }
</style>