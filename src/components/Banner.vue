<template>
  <div class="banner">
    <div class="container flex-center-between">
    <div class="item">
      <img src="../assets/img/buy-comics-digital-comics.png" alt="">
      <span>Digital Comics</span>
    </div>

    <div class="item">
      <img src="../assets/img/buy-comics-merchandise.png" alt="">
      <span>DC Merchandise</span>
    </div>

    <div class="item">
      <img src="../assets/img/buy-comics-subscriptions.png" alt="">
      <span>Subscription</span>
    </div>

    <div class="item">
      <img src="../assets/img/buy-comics-shop-locator.png" alt="">
      <span>Comic Shop Locator</span>
    </div>

    <div class="item">
      <img src="../assets/img/buy-dc-power-visa.svg" alt="">
      <span>DC Power Visa</span>
    </div>

    </div>
  </div>
</template>

<script>
export default {
  name: 'Banner'
}
</script>

<style lang="scss" scoped>
@import '../assets/styles/vars.scss';

.banner {
  height: 155px;
  width: 100%;
  background-color: $brand-color;

  .item {
    color: white;
    text-transform: uppercase;
    display: flex;
    align-items: center;
    img {
      height: 50px;
      margin-right: 20px;
    }
      &:last-child img{
        width: 50px;
      }
    
  }
}
</style>