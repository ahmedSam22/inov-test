<template>
<section class="container p-0">
  <div class="row">
      <div class="col-md-12 col-8 ">
     <div class="main">
    <div class="dot-pattern"></div>
    <div class="main__slider ">
        <img src="../assets/logo.png" height="100" alt="" srcset="">
        <div class="">
               <Slider />
        </div>
    </div>

    <div class="bg-circle"></div>
  </div>
  </div>
  </div>

    
</section>
 
</template>

<script>
  import Slider from './Slider.vue';

export default {
  components: {
    Slider,
  },
};
</script>

<style lang="scss" scoped>
@import url("../style/Global.scss");
.main {
  position: relative;
  // padding: 20px;
  display: flex;
  justify-content: center;
  height: 700px;
  align-items: center;
  @media (max-width:470px) {
    padding: 5px;
        width: auto;
  justify-content: start;

        height: 349.29px;
    }

  &__slider {
    width: 846.89px;
    height: 549.29px;
    background: #8d5da7;
    border-radius: 40px;
    z-index: 1;
    overflow: hidden;
    position: relative;
    @media (max-width:770px) {
        width: 450px;
        height: 349.29px;
    }
    img{
        position: absolute;
        top: calc(549 / 2) - 50px;
        left: calc(847 / 2) - 50px;
        opacity: .7;
        @media (max-width:770px) {
            display: none;
        }
    }
    &__layer{
        height: 100%;
        width: 100%;
        background: url("../assets/bg.jpg");
        background-size: cover;
    }

  }
}
.dot-pattern {
  position: absolute;
  left: 125px;
  top: 15px;
  @media (max-width : 1245px) {
      display: none;
  }
}

.bg-circle {
  position: absolute;
  right: 122px;
  bottom: -34px;
  @media (max-width : 1245px) {
      display: none;
  }
}
</style>