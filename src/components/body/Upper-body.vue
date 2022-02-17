<template>
  <section class="container p-0">
    <div class="row">
      <div class="col-md-12 col-8">
        <div class="main">
          <div class="dot-pattern"></div>
          <div class="main__slider">
            <video autoplay loop class="w-100">
              <source src="../../assets/upper.mp4" type="video/mp4" />
            </video>
          </div>
          <div class="bg-circle"></div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  components: {},
};
</script>

<style lang="scss" scoped>
@import url("../../style/Global.scss");
.main {
  position: relative;
  display: flex;
  justify-content: center;
  height: 700px;
  align-items: center;
  @media (max-width: 470px) {
    padding: 5px;
    width: auto;
    justify-content: start;
    height: 349.29px;
  }
  &__slider {
    width: 846.89px;
    height: min-content;
    background: #8d5da7;
    border-radius: 40px;
    z-index: 1;
    overflow: hidden;
    position: relative;
    @media (max-width: 770px) {
      width: 450px;
    }
  }
}
.dot-pattern {
  position: absolute;
  left: 125px;
  top: 15px;
  @media (max-width: 1245px) {
    display: none;
  }
}
.bg-circle {
  position: absolute;
  right: 122px;
  bottom: -15px;
  @media (max-width: 1245px) {
    display: none;
  }
}
</style>