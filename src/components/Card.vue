<template>

  <div>
    <img :src="card.thumb" :alt="card.series">
    <h4>
      {{card.series}}
    </h4>
  </div>
</template>

<script>


export default {
  name: "Card",
  props: {
    card: Object
  } 
}
</script>

<style lang="scss" scoped>

img, h4 {
  cursor: pointer;
}
img {
  height: 190px;
  width: 190px;
  object-fit: cover;
  object-position: center top;
}

h4 {
  margin: 20px 0;
}

</style>