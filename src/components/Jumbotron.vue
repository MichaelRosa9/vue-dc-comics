<template>

  <div class="jumbotron">
    <div class="container">
    <button>
      Current Series
    </button>
    </div>
  </div>

</template>

<script>


export default {
  name: 'Jumbotron',
}
</script>

<style lang="scss" scoped>

  @import "../assets/styles/vars.scss";

  .jumbotron {
    height: 400px;
    background-image: url('~@/assets/img/jumbotron.jpg');
    
    button {
      position: absolute;
      bottom: -25px;
      height: 55px;
      width: 250px;
      border: none;
      box-shadow: 0 0 2px #000000;
      font-size: 23px;
      font-weight: 600;
      color: white;
      text-transform: uppercase;
      background-color: $brand-color;
      cursor: pointer;

    }
  }
</style>>