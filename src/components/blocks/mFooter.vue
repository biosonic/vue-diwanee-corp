<template>
  <footer>
    <div class="b-contacts">
      <h5>Let's get connected</h5>
      <ul class='footer-social'>
        <li class="footer-social__item">
          <a href="mailto:info@diwanee.com" target='_blank'><img src='../../assets/img/footer/mail-ico--white.svg'></a>
        </li>
        <li class="footer-social__item">
          <a href="https://www.facebook.com/Diwanee" target='_blank'><img src='../../assets/img/footer/fb-ico.svg'></a>
        </li>
        <li class="footer-social__item">
          <a href="https://twitter.com/diwanee" target='_blank'><img src='../../assets/img/footer/twitt-ico.svg'></a>
        </li>
        <!-- <li class="footer-social__item">
        <a href="https://plus.google.com/+Diwanee-serbiaRs" target='_blank'><img src='../../assets/img/footer/gplus-ico.svg'></a>
      </li> -->
    </ul>

    <div class="b-contacts__item">
      <h4>Dubai</h4>
      <p>Office Park, Building Block A</p>
      <p>Units A301-A302</p>
      <p>Dubai Internet City</p>
      <p>T:971 4 - 434 7147</p>
    </div>
    <div class="b-contacts__item">
      <h4>Beirut</h4>
      <p>Beirut Digital District/BDD 1075</p>
      <p>2nd and 3rd floor</p>
      <p>Bechara El Khoury</p>
      <p>T:961 1 - 660327</p>
    </div>
    <div class="b-contacts__item">
      <h4>Belgrade</h4>
      <p>Resavska 23</p>
      <p>11000 Belgrade</p>
      <p>T:381 11 - 3340 117</p>
    </div>
  </div>
  <div class="footer-pre">
    <a href="http://fr.webedia-group.com/"><img src="../../assets/img/footer/webedia.svg" alt=""></a>
  </div>
  <div class="footer-copy">
    <p>Copyright &copy 2017 Diwanee All Rights resereved</p>
    <div v-on:click="toTop" class='bck-to-top'>back to top<img src="../../assets/img/footer/bcktotop.svg" alt=""></div>
  </div>
</footer>
</template>

<style lang="scss" scoped>

@function cvp($target, $container) {
  @return ($target / $container) * 100vw;
}
@function calculateRem($size) {
  $remSize: $size / $base__font-size;
  @return #{$remSize}rem;
}

@import "../../assets/sass/app.scss";

@import "../../assets/sass/base/breakpoints";
@import "../../assets/sass/base/mixins";
@import "../../assets/sass/base/typography";
@import "../../assets/sass/base/reset";

@import "../../assets/sass/b-contact";
@import "../../assets/sass/footer";
@import "../../assets/sass/sections";

footer {
  background: #f8f8f8;
  padding-top: 7%;
  font-weight: 400;
  line-height: 16px;
  p {
    line-height: 23px;
  }
  h1, h2, h3, h4, h5, h6 {
    font-family: $serif;
    line-height: 23px;
  }
  h4 {
    font-size: 23px;
    font-weight: 700;
  }
  .footer-copy {
      margin-bottom: 0;
      padding-bottom: 8%;
      p {
        line-height: 13px;
      }
  }
}

</style>

<script>

  export default {
    methods: {
      toTop: function(){
        window.scrollTo(0, 0);
      }
    }
  }
  
</script>
