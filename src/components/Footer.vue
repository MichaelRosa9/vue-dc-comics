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
              <a href="#">Characters</a>
            </li>
            <li>
              <a href="#">Comics</a>
            </li>
            <li>
              <a href="#">Movies</a>
            </li>
            <li>
              <a href="#">TV</a>
            </li>
            <li>
              <a href="#">Games</a>
            </li>
            <li>
              <a href="#">Videos</a>
            </li>
            <li>
              <a href="#">News</a>
            </li>
          </ul>

          <ul>
            <li class="title">
              DC
            </li>
            <li>
              <a href="#">Terms Of Use</a>
            </li>
            <li>
              <a href="#">Privacy policy&#40;New&#41;</a>
            </li>
            <li>
              <a href="#">Ad Chioices</a>
            </li>
            <li>
              <a href="#">Advertising</a>
            </li>
            <li>
              <a href="#">Jobs</a>
            </li>
            <li>
              <a href="#">Subscriptions</a>
            </li>
            <li>
              <a href="#">Talent Workshops</a>
            </li>
            <li>
              <a href="#">CPSC Certificates</a>
            </li>
            <li>
              <a href="#">Ratings</a>
            </li>
            <li>
              <a href="#">Shop Help</a>
            </li>
            <li>
              <a href="#">Contact Us</a>
            </li>
          </ul>

          <ul>
            <li class="title">
              Sites
            </li>
            <li>
              <a href="#">DC</a>
            </li>
            <li>
              <a href="#">MAD Magazine</a>
            </li>
            <li>
              <a href="#">DC Kids</a>
            </li>
            <li>
              <a href="#">DC Universe</a>
            </li>
            <li>
              <a href="#">DC Power Visa</a>
            </li>
          </ul>

          <ul>
            <li class="title">
              Shop
            </li>
            <li>
              <a href="#">Shop DC</a>
            </li>
            <li>
              <a href="#">Shop DC Collectibles</a>
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
    width: 470px;
    float: left;
  }

  ul {
    color: grey;
    float: left;
    padding-right: 45px;

    li {
      font-weight: 300;
      font-size: 13px;
      margin-bottom: 6px;
      white-space: nowrap;

      a {
        font-weight: 600;
        color: inherit;
      }
      a:hover {
        color: $brand-color
      }
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
    font-weight: 600;
    border: solid 2px $brand-color;
    color: white;
    cursor: pointer;

    &:hover {
      background-color: $brand-color;
      transition: background-color 300ms linear;
    }
  }

  h3 {
    color: $brand-color;
  }
  li {
    margin-left: 20px;
  }

  img:hover {
    opacity: .6;
    transition: opacity 1s;
  }
} //END footer-bottom
</style>
