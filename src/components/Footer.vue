<template>
  <footer>
  <div class="footer-top">
    <div class="container clear-fix">

      <div class="footer-list clear-fix">
        
        <ul>
          <li class="title">
            DC COMICS
          </li>
          <li>
            Characters
          </li>
          <li>
            Comics
          </li>
          <li>
            Movies
          </li>
          <li>
            TV
          </li>
          <li>
            Games
          </li>
          <li>
            Videos
          </li>
          <li>
            News
          </li>
        </ul>

        <ul>
          <li class="title">
            DC
          </li>
          <li>
            Terms Of Use
          </li>
          <li>
            Privacy policy&#40;New&#41;
          </li>
          <li>
            Ad Chioices
          </li>
          <li>
            Advertising
          </li>
          <li>
            Jobs
          </li>
          <li>
            Subscriptions
          </li>
          <li>
            Talent Workshops
          </li>
          <li>
            CPSC Certificates
          </li>
          <li>
            Ratings
          </li>
          <li>
            Shop Help
          </li>
          <li>
            Contact Us
          </li>
        </ul>

        <ul>
          <li class="title">
            Sites
          </li>
          <li>
            DC
          </li>
          <li>
            MAD Magazine
          </li>
          <li>
            DC Kids
          </li>
          <li>
            DC Universe
          </li>
          <li>
            DC Power Visa
          </li>        
        </ul>

        <ul>
          <li class="title">
            Shop
          </li>
          <li>
            Shop DC
          </li>
          <li>
            Shop DC Collectibles
          </li>        
        </ul>
      </div>
      <div class="box">
        <img src="" alt="">
      </div>
    </div>

  </div>

  <div class="footer-bottom"></div>
  </footer>
</template>

<script>


export default {
  name: 'Footer',  
  data(){
    return{
      
    }
  }
}
</script>


<style scoped lang="scss">

@import '../assets/styles/vars.scss';

.footer-top {
    height: 370px;
    width: 100%;
    background-image: url('~@/assets/img/footer-bg.jpg');
    background-size: cover;


  .footer-list {
    position: relative;
    padding-top: 20px;
    width: 450px;    
    float: left;
  }

  ul{
    color: grey;
    float: left;
    padding-right: 40px;

    li {
      font-weight: 300;
      font-size: 13px;
      margin-bottom: 6px;
      white-space:nowrap
    }
  }
  ul:last-child {    
      position: absolute;
      bottom: -20px;
  }
  .title {
    font-weight: 700;
    font-size: 18px;
    text-transform: uppercase;
    color: white;
    margin-bottom: 20px;
  }

  .box {
    height: 100%;
    width: 560px;
    float: right;
    margin-right: 25px;
    background-image: url('~@/assets/img/dc-logo-bg.png');
    background-size: cover;
    background-position: center;
  }
}
  
</style>
