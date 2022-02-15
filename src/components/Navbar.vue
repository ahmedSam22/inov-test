<template>
  <div>
    <section class="container">
      <ul class="d-flex w-100 d">
        <li>
          <img src="../assets/logo.png" alt="" />
        </li>
        <li><router-link to="/"></router-link> الرئيسية</li>
        <li><router-link to="/"></router-link> التصنيفات</li>
        <li><router-link to="/"></router-link> التطبيقات</li>
        <li><router-link to="/"></router-link> طور تطبيق</li>
      </ul>
    </section>
  </div>
</template>

<script>
export default {};
</script>
<style scoped lang="scss">
ul {
  list-style: none;
  align-items: center;
  padding: 0 177px; //to chamge .
  li {
    font-size: 18px;
    font-weight: 600;
    margin-left: 100px;
  }
}
</style>
