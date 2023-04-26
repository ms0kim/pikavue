<script>
  export default {
    data() {
      return {
        scrollPosition: null,
      }
    },
    methods: {
      updateScroll(){
        this.scrollPosition = window.scrollY
      },
    },
    mounted() {
      window.addEventListener('scroll', this.updateScroll);
    },
  }
</script>

<template>
  <ul :class="{nav: scrollPosition < 1, navActive: scrollPosition > 1}">
    <li>
      <div class="logo"><img src="../assets/media/pikavue_logo.svg" alt=""></div>
      <div>가격 안내<span>10% 할인중</span></div>
      <div>가이드</div>
    </li>
    <li>
      <button class="login">로그인</button>
      <button class="small">무료로 사용하기</button>
    </li>
  </ul>
</template>