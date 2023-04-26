<script>
  import { ImgComparisonSlider } from '@img-comparison-slider/vue';

  export default {
    components: {
      ImgComparisonSlider,
    },
  }
</script>

<template>
  <div class="imageUp">
    <div>
      <h3>AI 이미지 업스케일링</h3>
      <h5>크고 선명한 이미지로 업스케일링 하세요</h5>
      <button>더 알아보기</button>
  
      <div>
        <div class="txt">
          <h5>이미지 업스케일링</h5>
          <p>이미지를 2~4배까지 선명하게 업스케일링 할 수 있습니다</p>
        </div>
        <ImgComparisonSlider 
          hover="hover"
          class="imgSlide"
        >
          <!-- eslint-disable -->
          <img
            slot="first"
            src="../../assets/media/cat low.jpg"
          />
          <img
            slot="second"
            src="../../assets/media/cat.jpg"
          />
          <!-- eslint-enable -->
        </ImgComparisonSlider>
      </div>
      <ul class="imgLs">
        <li>
          <div class="txt">
            <h5>노출 필터</h5>
            <p>어두운 이미지를 밝게 조절할 수 있습니다</p>
          </div>
          <ImgComparisonSlider 
            hover="hover"
            class="imgSlide"
          >
            <!-- eslint-disable -->
            <img
              slot="first"
              src="../../assets/media/spring.jpg"
            />
            <img
              slot="second"
              src="../../assets/media/spring-after.jpg"
            />
            <!-- eslint-enable -->
          </ImgComparisonSlider>
        </li>
        <li>
          <div class="txt">
            <h5>색조 필터</h5>
            <p>색감이 부족한 이미지의 색조를 높힐 수 있습니다</p>
          </div>
          <ImgComparisonSlider 
            hover="hover"
            class="imgSlide"
          >
            <!-- eslint-disable -->
            <img
              slot="first"
              src="../../assets/media/summer.jpg"
            />
            <img
              slot="second"
              src="../../assets/media/summer-after.jpg"
            />
            <!-- eslint-enable -->
          </ImgComparisonSlider>
        </li>
        <li>
          <div class="txt">
            <h5>채도 필터</h5>
            <p>이미지를 채도를 조절할 수 있습니다</p>
          </div>
          <ImgComparisonSlider 
            hover="hover"
            class="imgSlide"
          >
            <!-- eslint-disable -->
            <img
              slot="first"
              src="../../assets/media/fall.jpg"
            />
            <img
              slot="second"
              src="../../assets/media/fall-after.jpg"
            />
            <!-- eslint-enable -->
          </ImgComparisonSlider>
        </li>
        <li>
          <div class="txt">
            <h5>선명한 필터</h5>
            <p>이미지의 선명도를 조절할 수 있습니다</p>
          </div>
          <ImgComparisonSlider 
            hover="hover"
            class="imgSlide"
          >
            <!-- eslint-disable -->
            <img
              slot="first"
              src="../../assets/media/winter.jpg"
            />
            <img
              slot="second"
              src="../../assets/media/winter-after.jpg"
            />
            <!-- eslint-enable -->
          </ImgComparisonSlider>
        </li>
      </ul>
    </div>
  </div>
</template>