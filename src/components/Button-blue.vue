<template>

  <button>
      {{button_text}}
    </button>

</template>

<script>
export default {
  name: 'Button',
  props: {
    button_text: Object
  }
}
</script>

<style lang="scss" scoped>

  @import "../assets/styles/vars.scss";

  button {
        
        border: none;
        box-shadow: 0 0 2px #000000;
        font-weight: 600;
        color: white;
        text-transform: uppercase;
        background-color: $brand-color;
        cursor: pointer;

  }

</style>