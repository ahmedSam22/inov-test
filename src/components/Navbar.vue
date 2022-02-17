<template>
  <div>
    <section class="container">
      <ul class="w-100 toResponsive" id="forToggle">
        <li>
          <img src="../assets/logo.png" alt="" />
        </li>
        <li><router-link to="/"></router-link> الرئيسية</li>
        <li><router-link to="/"></router-link> التصنيفات</li>
        <li><router-link to="/"></router-link> التطبيقات</li>
        <li><router-link to="/"></router-link> طور تطبيق</li>
      </ul>
    </section>
    <div class="accordion w-100" id="accordionExample">
      <div class="accordion-item">
        <h2 class="accordion-header" id="headingOne">
          <span
            class="accordion-button collapsed"
            data-bs-toggle="collapse"
            data-bs-target="#collapseOne"
            aria-expanded="true"
            aria-controls="collapseOne"
          >
            <img src="../assets/logo.png" alt="" />
          </span>
        </h2>
        <div
          id="collapseOne"
          class="accordion-collapse collapse"
          aria-labelledby="headingOne"
          data-bs-parent="#accordionExample"
        >
          <div class="accordion-body">
            <ul class="w-100">
              <li><router-link to="/"></router-link> الرئيسية</li>
              <li><router-link to="/"></router-link> التصنيفات</li>
              <li><router-link to="/"></router-link> التطبيقات</li>
              <li><router-link to="/"></router-link> طور تطبيق</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>


<style scoped lang="scss">
.toResponsive {
  display: flex;
  list-style: none;
  align-items: center;
  padding: 0 177px; //to chamge .
  @media (max-width: 1245px) {
    padding: 0;
  }
  @media (max-width: 445px) {
    display: none;
  }
  li {
    font-size: 18px;
    font-weight: 600;
    margin-left: 100px;
    @media (max-width: 800px) {
      margin-left: 30px;
      font-size: 14px;
    }
  }
}
.accordion {
  width: 100% !important;
  @media (min-width: 445px) {
    display: none;
  }
  ul {
    list-style: none;
    line-height: 20px;
    li {
      text-align: right;
    }
  }
}
</style>

<script >
export default {
  data() {
    return {
      toggle: false,
    };
  },
};
</script>