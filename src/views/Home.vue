<script setup lang="ts">
import Footer from '../components/layouts/Footer/Footer.vue'
import AboutUs from '../components/layouts/AboutUs.vue'
</script>

<style lang="scss" scoped>
.banner {
  background-image: url('../assets/images/banner_top.png');
  height: 700px;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;

  img {
    width: 974px;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translateX(-50%) translateY(-50%);
    margin-top: 30px;
  }

  @media screen and (max-width: 425px) {
    height: auto;
    background-repeat: no-repeat;
    background-size: cover;
    position: relative;
    margin-top: 56px;
    img {
      width: 100%;
      position: initial;
      transform: translateX(0) translateY(0);
    }
  }
}

.info-container {
  position: relative;

  .info-box {
    padding-top: 30px;
  }

  .info-box img {
    width: 100%;
  }

  .info-box .blue_text {
    font-weight: 800;
    font-size: 96px;
    line-height: 117px;
    text-align: center;
    text-transform: uppercase;
    color: #BBD7FE;
  }
}


.featured-container {
  padding-top: 300px;

  .featured-box {
    .feature_title {
      margin-bottom: 15px;
      font-weight: 600;
      font-size: 24px;
      line-height: 29px;
    }

    .feature_highlight {
      font-size: 28px;
      margin-bottom: 20px;
    }

    .featured-des {

    }
  }

  .featured-circle {
    position: relative;

    .btn_box_top, .btn_box_center, .btn_box_bottom {
      .btn_box_left {
        text-align: left;
      }

      .btn_box_right {
        text-align: right;
      }
    }

    .bnt_box {
      text-align: center;
      margin: 55px 0;
    }

    .btn_box_center {
      width: 96%;
      margin: 0 auto;
    }

    .btn_box_top, .btn_box_bottom {
      width: 75%;
      margin: 0 auto;
    }

    .featured-circle-logo {
      position: absolute;
      left: 50%;
      top: 50%;
      transform: translateX(-50%) translateY(-50%);
      z-index: 1;
    }

    .featured-circle-layer {
      position: absolute;
      left: 50%;
      top: 50%;
      //transform: translateX(-50%) translateY(-50%);
      margin-top: -350px;
      margin-left: -340px;
    }
  }
}
</style>

<template>
  <div id="banner" class="banner container-fluid">
    <img src="@/assets/images/financial_free.png" alt="">
  </div>
  <div id="info-container">
    <div class="info-box container">
      <div class="row">
        <div class="col-md-6">
          <div class="info-content left-info">
            <div>
              <h2>Give people freedom</h2>
              <div class="info-des">
                <p>Our goal is "Give People Freedom", with a mission to create innovative services that do not exist yet
                  in the world.</p>
                <p>We have already started and will continue to give people various opportunities to grow their
                  financial assets. Eventually, we would like them to independently manage their assets effectively and
                  successfully after partnering with us. </p>
                <p>We believe that if we can contribute to helping people gain more financial freedom, collaboratively,
                  we can change the world as much as possible. </p>
              </div>
            </div>
          </div>
        </div>
        <div class="col-md-6">
          <div><img style="max-width: 516px;" src="@/assets/images/yacht.png" alt=""></div>
        </div>
      </div>
    </div>
    <div class="info-box container reveal">
      <div class="row">
        <div class="col-md-6 left-info">
          <div><img style="max-width: 408px;" src="@/assets/images/invest.png" alt=""></div>
        </div>
        <div class="col-md-6">
          <div class="info-content">
            <div>
              <h2>Vision & Mission</h2>
              <div class="info-des">
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec interdum risus at ligula vehicula
                  egestas. In ut justo pharetra, faucibus diam id, aliquet turpis. Proin vitae libero sit amet justo
                  porttitor sollicitudin. Sed eu posuere tellus. In facilisis volutpat risus id tristique. Sed in diam
                  condimentum enim rhoncus congue. Praesent scelerisque purus et libero sollicitudin blandit.</p>
                <p>Vestibulum feugiat augue sit amet imperdiet viverra. Donec iaculis tempus enim a gravida. Aenean
                  consectetur ex in scelerisque gravida. Nulla ultrices metus tortor, ut egestas orci rhoncus eget. Nunc
                  hendrerit ligula sit amet nisl scelerisque, nec porta velit vulputate. Donec molestie id lorem quis
                  vulputate. Praesent sed urna vitae sapien vehicula consequat eu quis magna. Aliquam id lobortis
                  sapien. Morbi elit ante, fringilla at velit tincidunt, aliquam imperdiet justo. Nam aliquam varius
                  vulputate. Quisque dolor lacus, laoreet at eros ut, imperdiet ornare tortor. Curabitur auctor id lorem
                  sagittis dictum.</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="info-box container reveal">
      <div class="row">
        <div class="col-md-6">
          <div class="info-content left-info">
            <div>
              <h2>Why join us?</h2>
              <div class="info-des">
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec interdum risus at ligula vehicula
                  egestas.</p>
                <p>Vestibulum feugiat augue sit amet imperdiet viverra. Donec iaculis tempus enim a gravida. Aenean
                  consectetur ex in scelerisque gravida. Nulla ultrices metus tortor, ut egestas orci rhoncus eget.</p>
                <p>Nunc hendrerit ligula sit amet nisl scelerisque, nec porta velit vulputate. Donec molestie id lorem
                  quis vulputate. Praesent sed urna vitae sapien vehicula consequat eu quis magna. Aliquam id lobortis
                  sapien.</p>
                <p>Morbi elit ante, fringilla at velit tincidunt, aliquam imperdiet justo. Nam aliquam varius vulputate.
                  Quisque dolor lacus, laoreet at eros ut, imperdiet ornare tortor. Curabitur auctor id lorem sagittis
                  dictum.</p>
              </div>
            </div>
          </div>
        </div>
        <div class="col-md-6">
          <div><img style="max-width: 624px;" src="@/assets/images/building.png" alt=""></div>
        </div>
      </div>
    </div>
  </div>
  <div class="footer-banner">
    <div id="featured-container" class="container-fluid featured-container">
      <div class="container">
        <div class="featured-box">
          <div class="reveal">
            <p class="feature_title">Featured</p>
            <h2 class="feature_highlight header_title">TJEX ECOSYSTEM</h2>
            <div class="featured-des">
              <p>The TJex ecosystem employs a business ecosystem structure that provides interconnected services and
                helps our customers increase their value by accumulating business experiences using our platform.</p>
              <p>Our services comprise of four categories namely: the Financial Services for Retail Clients (tjex.fund,
                tjex.trade, tjex.digital), tools for further assistance to clients/users ( tjex.help, tjex.ai), Human
                Resources Management with unique referral recruitment system feature (tjex.org), Real Estate Investment
                Trust (REIT) which is an affordable investment opportunity (tjex.estate), and CRM (Customer Relationship
                Management) development solutions for start-up companies (tjex.cloud) </p>
            </div>
          </div>
          <div class="featured-circle reveal">
            <img class="featured-circle-logo" src="@/assets/images/featured_logo.png" alt="">
            <img class="featured-circle-layer" src="@/assets/images/featured_layer.png" alt="">
            <div class="">
              <div class="row">
                <div class="col-12 text-center bnt_box">
                  <button class="btn blue_btn">TJex.fund</button>
                </div>
              </div>
              <div class="row btn_box_top">
                <div class="col-md-6 bnt_box btn_box_left">
                  <button class="btn blue_btn">TJex.trade</button>
                </div>
                <div class="col-md-6 bnt_box btn_box_right">
                  <button class="btn blue_btn">TJex.digital</button>
                </div>
              </div>
              <div class="row btn_box_center">
                <div class="col-md-6 bnt_box btn_box_left">
                  <button class="btn blue_btn">TJex.help</button>
                </div>
                <div class="col-md-6 bnt_box btn_box_right">
                  <button class="btn blue_btn">TJex.ai</button>
                </div>
              </div>
              <div class="row btn_box_bottom">
                <div class="col-md-6 bnt_box btn_box_left">
                  <button class="btn blue_btn">TJex.estate</button>
                </div>
                <div class="col-md-6 bnt_box btn_box_right">
                  <button class="btn blue_btn">TJex.org</button>
                </div>
              </div>
              <div class="row">
                <div class="col-12 bnt_box">
                  <button class="btn blue_btn">TJex.clound</button>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <AboutUs/>
    <Footer/>
  </div>

</template>
