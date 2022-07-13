<script>
export default {
  name: 'Footer',
}
</script>
<style lang="scss">
@import 'footer';
</style>
<template>
  <div id="footer">
    <div class="container">
      <div class="footer-box">
        <div class="row">
          <div class="col-sm-8">
            <div><img src="@/assets/images/logo.png" alt=""> <span class="copyright">Copyright @ 2018-2022 TJTECH Company SL.All rights reserved</span>
            </div>
          </div>
          <div class="col-sm-4 text-right">
            <div class="social_group_ic">
              <img src="@/assets/images/twitter_ic.png" alt="">
              <img src="@/assets/images/fb_ic.png" alt="">
              <img src="@/assets/images/linkedin_ic.png" alt="">
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
