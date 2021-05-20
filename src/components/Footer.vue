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
          <img src="" alt="" />
        </div>
      </div>
    </div>

    <div class="footer-bottom">
      <div class="container flex-center-between">
        <button type="button">SIGN-UP NOW!</button>

        <div class="social-media flex-center-between">
          <h3>
            FOLLOW US
          </h3>

          <ul class="social-links flex-center-between">
            <li>
              <a href="#"
                ><img src="../assets/img/footer-facebook.png" alt=""
              /></a>
            </li>
            <li>
              <a href="#"><img src="../assets/img/footer-twitter.png" alt=""/></a>
            </li>
            <li>
              <a href="#"><img src="../assets/img/footer-youtube.png" alt=""/></a>
            </li>
            <li>
              <a href="#"
                ><img src="../assets/img/footer-pinterest.png" alt=""
              /></a>
            </li>
            <li>
              <a href="#"
                ><img src="../assets/img/footer-periscope.png" alt=""
              /></a>
            </li>
          </ul>
        </div>      
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
  data() {
    return {};
  },
};
</script>

<style scoped lang="scss">
@import "../assets/styles/vars.scss";

.footer-top {
  height: 370px;
  width: 100%;
  background-image: url("~@/assets/img/footer-bg.jpg");
  background-size: cover;

  .footer-list {
    position: relative;
    padding-top: 20px;
    width: 450px;
    float: left;
  }

  ul {
    color: grey;
    float: left;
    padding-right: 40px;

    li {
      font-weight: 300;
      font-size: 13px;
      margin-bottom: 6px;
      white-space: nowrap;
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
    background-image: url("~@/assets/img/dc-logo-bg.png");
    background-size: cover;
    background-position: center;
  }
} //END footer-top

.footer-bottom {
  height: 110px;
  background-color: #2a2a2a;
  text-transform: uppercase;
  
  button {
    background-color: inherit;
    padding: 10px;
    border: solid 2px $brand-color;
    color: white;
  }

  h3 {
    color: $brand-color;
  }
  li {
    margin-left: 20px;
  }
}
</style>
