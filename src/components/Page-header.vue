<template>
  <Navbar class="mb-5 w-100" />
  <div class="container">
    <div class="row">
      <div class="page--header text-lg-center col-12">
        <h1 class="mt-5">طور متجرك ووسع آفاق تجارتك مع سوق تطبيقات زد</h1>
        <p>
          طوّر تجارتك من خلال تطبيقات و حلول سوق تطبيقات زد التي تساعدك في نمو
          أرباحك عبر إدارة عمليات متجرك بشكل فعّال و احترافي
        </p>
        <button class="btn page--header__btn-custom">
          تصفّح التطبيقات
          <i class="fa-solid fa-angle-left pe-2"></i>
        </button>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
.page--header {
  display: grid;
  gap: 30px;
  @media (max-width: 575px) {
    display: flex;
    flex-wrap: wrap;
  }
  h1 {
    color: #8d5da7;
    font-weight: bolder;
    margin: 0;
    @media (max-width: 575px) {
      width: 60%;
    }
  }
  p {
    width: 38%;
    margin: auto;
    font-weight: 500;
    font-size: 18px;
    color: #111;
    line-height: 34px;
    @media (max-width: 575px) {
      margin: 0;
      width: 60%;
    }
  }
  &__btn-custom {
    width: 295px;
    height: 60px;
    background: #8d5da7;
    color: #fdb515;
    font-size: 18px;
    margin: auto;
    &:hover {
      color: white;
    }
    @media (max-width: 575px) {
      margin: 0;
    }
  }
}
</style>

<script>
import Navbar from "./Navbar.vue";
export default {
  components: {
    Navbar,
  },
};
</script>
