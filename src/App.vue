<template>
  <div id="app">

    <Header class="container flex-center-between" />
    <Jumbotron />
    <Main class="" />
    <Banner />
    <Footer class="" />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Jumbotron from './components/Jumbotron.vue'
import Main from './components/Main.vue'
import Banner from './components/Banner.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer,
    Jumbotron,
    Banner
  }  
}
</script>

<style lang="scss">
@import './assets/styles/general.scss';
@import './assets/styles/utilities.scss';

</style>
