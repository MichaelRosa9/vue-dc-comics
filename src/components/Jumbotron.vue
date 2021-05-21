<template>

  <div class="jumbotron">
    <div class="container">
      <Button class="button" :button_text="text"/>
    
    </div>
  </div>

</template>

<script>
import Button from './Button-blue.vue'

export default {
  name: 'Jumbotron',
  components: {
    Button
  },
  data(){
    return{
      text: 'current series'
    }
  }
}
</script>

<style lang="scss" scoped>

  @import "../assets/styles/vars.scss";

  .jumbotron {
    height: 400px;
    background-image: url('~@/assets/img/jumbotron.jpg');
    
    .button {
      position: absolute;
      bottom: -25px;
      height: 55px;
      width: 250px;     
      box-shadow: 0 0 2px #000000;
      font-size: 23px;
    }
  }
</style>>