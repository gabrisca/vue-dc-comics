<template>
  <div id="app">
    <HeaderComp />
    <Main />
    <Footer />
  </div>
</template>

<script>
import Footer from './components/Footer.vue'
import HeaderComp from './components/HeaderComp.vue'
import Main from './components/Main.vue'


export default {
  name: 'App',
  components: {
    HeaderComp,
    Main,
    Footer,
  }
}
</script>


<style lang="scss">
@import './assets/style/general.scss';
@import './assets/style//utilities.scss';
</style>
