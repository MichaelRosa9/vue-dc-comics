<template>
  <div id="app">

    <Header class="container flex-center-between" />
    <Jumbotron />
    <Main class="" />
    <Footer class="" />

  </div>
</template>

<script>
import Header from './components/Header.vue'
import Jumbotron from './components/Jumbotron.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer,
    Jumbotron
  }  
}
</script>

<style lang="scss">
@import './assets/styles/general.scss';
@import './assets/styles/utilities.scss';

</style>
