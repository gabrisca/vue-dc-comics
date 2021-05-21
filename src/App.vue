<template>
  <div id="app">
    <HeaderComp />
    <Jumbotron />
    <Main />
    <BlueBand />
    <Footer />
  </div>
</template>

<script>
import HeaderComp from './components/HeaderComp.vue'
import Jumbotron from './components/Jumbotron.vue'
import Main from './components/Main.vue'
import BlueBand from './components/BlueBand.vue'
import Footer from './components/Footer.vue'


export default {
  name: 'App',
  components: {
    HeaderComp,
    Jumbotron,
    Main,
    BlueBand,
    Footer,
  }
}
</script>


<style lang="scss">
@import './assets/style/general.scss';
@import './assets/style//utilities.scss';
</style>
