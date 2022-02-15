<template>
  <div class="footer ">
    <div class="footer__contact text-center container">
      <img src="../assets/logo.png" alt="" />
      <ul class="d-flex justify-content-center">
        <li v-for="(icon,index) of icons" :key="index">
          <i :class="icon" class="ms-4"></i>
        </li>
      </ul>
    </div>
    <div class="footer__chat d-flex justify-content-between p-3">
      <span>
        <i class="fa-solid fa-comments"></i>
      </span>
      <span> <i class="fa-solid fa-arrow-up up"></i></span>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.footer {
  background: #835d9d;
  &__contact {
    img {
      height: 70px;
      width: 150px;
    }
  }
  ul {
    list-style: none;
    li {
      color: white;
      font-size: 20px;
    }
  }
  &__chat {
        align-items: baseline;

    svg {
      background: #fdb515;
      color: #835d9d;
      border-radius: 50%;
      font-size: 30px;
      padding: 10px;
          }
          .up{
            font-size: 20px;
          }
  }
}
</style>

<script>
export default {
  data() {
    return {
      icons: [
        "fa-brands fa-twitter",
        "fa-brands fa-instagram",
        "fa-brands fa-linkedin-in",
        "fa-brands fa-youtube",
      ],
    };
  },
};
</script>