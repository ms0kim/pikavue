<script>
  import { Autoplay } from 'swiper';
  import { Swiper, SwiperSlide } from 'swiper/vue';
  import 'swiper/css'

  export default {
    components: {
      Swiper,
      SwiperSlide,
    },
    setup() {
      const onSwiper = (swiper) => {
        console.log(swiper);
      };
      const onSlideChange = () => {
        console.log('slide change');
      };
      return {
        onSwiper,
        onSlideChange,
        modules: [Autoplay],
      };
    },
  }
</script>

<template>
  <div class="sub">
    <div>
      <h4>4K 시대에 맞춰야 하는 미디어</h4>
      <h4>선명한 업스케일링과 다양한 필터까지!</h4>
      <swiper
        :modules="modules"
        :speed="8000"
        :loop="true"
        :centeredSlides="true"
        :autoplay="{
          delay: 0,
          disableOnInteraction: false,
          pauseOnMouseEnter: true,
        }"
        :slidesPerView="4.8"
        :spaceBetween="20"
        :slidesPerGroup="1"
        :pagination="{
          clickable: false,
        }"
        class="subSlide"
      >
        <swiper-slide class="slide">
          <img src="../../assets/media/cat.jpg" alt="">
          <p>
            <span>이미지</span>
            <b>해상도가 낮은 이미지를 선명하게</b>
            <b>2~4배로 업스케일링 할 수 있어요</b>
          </p>
        </swiper-slide>
        <swiper-slide class="slide">
          <img src="../../assets/media/spring-after.jpg" alt="">
          <p>
            <span>이미지</span>
            <b>노출 필터로 어두운 이미지를</b>
            <b>밝게 조절할 수 있어요</b>
          </p>
        </swiper-slide>
        <swiper-slide class="slide">
          <img src="../../assets/media/summer-after.jpg" alt="">
          <p>
            <span>이미지</span>
            <b>색조 필터로 색감이 부족한 이미지를</b>
            <b>다채롭게 조절할 수 있어요</b>
          </p>
        </swiper-slide>
        <swiper-slide class="slide">
          <img src="../../assets/media/fall-after.jpg" alt="">
          <p>
            <span>이미지</span>
            <b>채도 필터로 이미지의 색감을</b>
            <b>흑백까지 조절할 수 있어요</b>
          </p>
        </swiper-slide>
        <swiper-slide class="slide">
          <img src="../../assets/media/winter-after.jpg" alt="">
          <p>
            <span>이미지</span>
            <b>선명한 필터로 흐릿한 이미지를</b>
            <b>더 선명하게 조절할 수 있어요</b>
          </p>
        </swiper-slide>
        <swiper-slide class="slide">
          <img src="../../assets/media/cat.jpg" alt="">
          <p>
            <span>동영상</span>
            <b>해상도가 낮은 동영상을</b>
            <b>선명하게 업스케일링 할 수 있어요</b>
          </p>
        </swiper-slide>
        <swiper-slide class="slide">
          <img src="../../assets/media/cat.jpg" alt="">
          <p>
            <span>이미지</span>
            <b>해상도가 낮은 이미지를 선명하게</b>
            <b>2~4배로 업스케일링 할 수 있어요</b>
          </p>
        </swiper-slide>
        <swiper-slide class="slide">
          <img src="../../assets/media/spring-after.jpg" alt="">
          <p>
            <span>이미지</span>
            <b>노출 필터로 어두운 이미지를</b>
            <b>밝게 조절할 수 있어요</b>
          </p>
        </swiper-slide>
        <swiper-slide class="slide">
          <img src="../../assets/media/summer-after.jpg" alt="">
          <p>
            <span>이미지</span>
            <b>색조 필터로 색감이 부족한 이미지를</b>
            <b>다채롭게 조절할 수 있어요</b>
          </p>
        </swiper-slide>
        <swiper-slide class="slide">
          <img src="../../assets/media/fall-after.jpg" alt="">
          <p>
            <span>이미지</span>
            <b>채도 필터로 이미지의 색감을</b>
            <b>흑백까지 조절할 수 있어요</b>
          </p>
        </swiper-slide>
        <swiper-slide class="slide">
          <img src="../../assets/media/winter-after.jpg" alt="">
          <p>
            <span>이미지</span>
            <b>선명한 필터로 흐릿한 이미지를</b>
            <b>더 선명하게 조절할 수 있어요</b>
          </p>
        </swiper-slide>
        <swiper-slide class="slide">
          <img src="../../assets/media/cat.jpg" alt="">
          <p>
            <span>동영상</span>
            <b>해상도가 낮은 동영상을</b>
            <b>선명하게 업스케일링 할 수 있어요</b>
          </p>
        </swiper-slide>
      </swiper>
    </div>
  </div>
</template>