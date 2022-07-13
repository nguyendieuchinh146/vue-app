<script>
export default {
  name: 'AboutUs',
}
</script>
<style lang="scss">
.about-us-container {
  margin-top: 30px;
  padding-top: 80px;
  position: relative;
  overflow: hidden;

  .whale-logo {
    position: absolute;
  }

  .about-us-box {
    .header_title {
      font-weight: 600;
      font-size: 48px;
      line-height: 58px;
      @media screen and(max-width: 425px) {
        font-size: 30px;
      }
    }

    .about-us-des {
      margin: 40px 0 40px 80px;
    }

    .about-us-menu {
      padding: 30px 0;

      h3 {
        font-size: 18px;
        font-weight: 600;
        color: #fff;
      }

      ul {
        padding: 0;
        margin: 0;

        li {
          list-style: none;
          padding: 5px 0;
          font-size: 12px;

          a {
            color: #e1e2e5;
          }
        }
      }
    }
  }
}
</style>
<template>
  <div id="about-us-container" class="reveal about-us-container">
    <!-- <img class="whale-logo" src="@/assets/images/whale.png" alt=""> -->
    <div class="about-us-box container">
      <h2 class="header_title">MORE ABOUT USE</h2>
      <div class="row">
        <div class="col-sm-7">
          <div class="about-us-des">
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et
              dolore
              magna aliqua. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut
              labore et dolore magna aliqua. </p>
            <button class="bnt blue_bd_btn">CONTACT US</button>
          </div>
        </div>
      </div>
      <div class="about-us-menu">
        <div class="row">
          <div class="col-sm-3 col-6">
            <h3>ABOUT US</h3>
            <ul>
              <li><a href="">About us</a></li>
              <li><a href="">Vision & Mission</a></li>
              <li><a href="">Our Culture</a></li>
              <li><a href="">Company Structure</a></li>
            </ul>
          </div>
          <div class="col-sm-3 col-6">
            <h3>USEFUL INFO</h3>
            <ul>
              <li><a href="">Careers</a></li>
              <li><a href="">Blog</a></li>
              <li><a href="">Contact Us</a></li>
              <li><a href="">Support</a></li>
            </ul>
          </div>
          <div class="col-sm-3 col-6">
            <h3>Legal</h3>
            <ul>
              <li><a href="">Legal</a></li>
              <li><a href="">Term & Conditions</a></li>
              <li><a href="">License Agreement</a></li>
              <li><a href="">Privacy policy</a></li>
            </ul>
          </div>
          <div class="col-sm-3 col-6"></div>
        </div>
      </div>
    </div>

  </div>
</template>
