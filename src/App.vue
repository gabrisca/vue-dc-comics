<template>
  <div id="app">
    <HeaderComp />
    <Main />
  </div>
</template>

<script>
import HeaderComp from './components/HeaderComp.vue'
import Main from './components/Main.vue'


export default {
  name: 'App',
  components: {
    HeaderComp,
    Main,
  }
}
</script>


<style lang="scss">
@import './assets/style/general.scss';
@import './assets/style//utilities.scss';
</style>
