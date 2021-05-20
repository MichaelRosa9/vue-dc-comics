<template>
  <div id="app">

    <Header class="container flex-center-between" />

  </div>
</template>

<script>
import Header from './components/Header.vue'

export default {
  name: 'App',
  components: {
    Header
  }
}
</script>

<style lang="scss">
@import './assets/styles/general.scss';
@import './assets/styles/utilities.scss';

</style>
