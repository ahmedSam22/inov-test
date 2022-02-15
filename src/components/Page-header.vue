<template>
  <div class="page--header text-center">
    <Navbar class="mb-3" />

    <h1>طور متجرك ووسع آفاق تجارتك مع سوق تطبيقات زد</h1>
    <p>
      طوّر تجارتك من خلال تطبيقات و حلول سوق تطبيقات زد التي تساعدك في نمو
      أرباحك عبر إدارة عمليات متجرك بشكل فعّال و احترافي
    </p>
    <button class="btn page--header__btn-custom">
      تصفّح التطبيقات
      <i class="fa-solid fa-angle-left pe-2"></i>
    </button>
  </div>
</template>

<style scoped lang="scss">
.page--header {
  display: grid;
  gap: 30px;
  h1 {
    color: #8d5da7;
    font-weight: bolder;
    margin: 0;
  }
  p {
    width: 38%;
    margin: auto;
    font-weight: 500;
    font-size: 18px;
    color: #111;
    line-height: 34px;
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
