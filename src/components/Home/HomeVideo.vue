<script>
  export default {
    data() {
      return {
        btn1: true,
        btn2: false,
      }
    },
    methods: {
      btn1Click() {
        this.btn1 = true;
        if(this.btn1){
          this.btn2 = false;
        }
      },
      btn2Click() {
        this.btn2 = true;
        if(this.btn2){
          this.btn1 = false;
        }
      }
    }
  }
</script>

<template>
  <div class="videoUp">
    <div>
      <h3>AI 동영상 업스케일링</h3>
      <h5>현실감을 선택하여 업스케일링 하세요</h5>
      <button>더 알아보기</button>
  
      <div class="videoLs">
        <div v-show="btn1">
          <video muted autoplay loop>
            <source src="../../assets/media/before.mp4" type="video/mp4">
            <strong>Your browser does not support the video tag.</strong>
          </video>
        </div>
        <div v-show="btn2">
          <video muted autoplay loop>
            <source src="../../assets/media/after.mp4" type="video/mp4">
            <strong>Your browser does not support the video tag.</strong>
          </video>
        </div>
        <div class="videoBtn">
          <div>
            <button id="video1" :class="{active : btn1}" @click="btn1Click">현실적</button>
            <label class="btnImg" :class="{active : btn1}" @click="btn1Click" for="video1"><img src="" alt=""></label>
          </div>
          <div>
            <button id="video2" :class="{active : btn2}" @click="btn2Click">비현실적</button>
            <label class="btnImg" :class="{active : btn2}" @click="btn2Click" for="video2"><img src="" alt=""></label>
          </div>
        </div>
        <div class="list" v-show="btn1">
          <h5>현실적인 동영상 업스케일링</h5>
          <p>현실적인 동영상으로 업스케일링 할 수 있습니다</p>
        </div>
        <div class="list" v-show="btn2">
          <h5>비현실적인 동영상 업스케일링</h5>
          <p>비현실적인 동영상으로 업스케일링 할 수 있습니다</p>
        </div>
      </div>
    </div>
  </div>
</template>