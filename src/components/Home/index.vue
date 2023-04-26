<script>
  import HeaderNav from '../HeaderNav.vue'
  import HomeMain from './HomeMain.vue'
  import HomeSub from './HomeSub.vue'
  import HomeImg from './HomeImg.vue'
  import HomeVideo from './HomeVideo.vue'
  import HomeAi from './HomeAi.vue'
  import HomePricing from './HomePricing.vue'
  import HomeStart from './HomeStart.vue'
  import HomeService from './HomeService.vue'
  import BottomFooter from '../BottomFooter.vue'


  export default {
    data() {
      return {
      }
    },
    components: {
      HeaderNav,
      HomeMain,
      HomeSub,
      HomeImg,
      HomeVideo,
      HomeAi,
      HomePricing,
      HomeStart,
      HomeService,
      BottomFooter,
    },
  };
</script>

<template>
  <div class="wrap">

    <div class="header">
      <HeaderNav />
      <HomeMain />
    </div>

    <HomeSub />
    <HomeImg />
    <HomeVideo />
    <HomeAi />
    <HomePricing />
    <HomeStart />
    <HomeService />
    <BottomFooter />

  </div>
</template>
