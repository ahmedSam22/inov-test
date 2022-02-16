<template>

  <div class="footer ">
    <div class="footer__contact text-center container ">
      <img src="../assets/logo.png" alt="" />
      <ul class="d-flex ">
        <li v-for="(icon,index) of icons" :key="index">
          <i :class="icon" class="ms-4"></i>
        </li>
      </ul>
    </div>
    <div class="footer__chat d-flex justify-content-between p-3">
      <span class="me-sm-1">
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
    @media (max-width:420px) {
      display: flex;
      flex-direction: column;
      width: 60%;
      margin: 0;
    }
    img {
      height: 70px;
      width: 150px;
      background-color: #f7f7f7;
      margin-top: 10px;
      border-top-left-radius: 20%;
      border-bottom-right-radius: 20%;
      @media (max-width:420px) {
  
      margin: auto;
      
    }
    }
  }
  ul {
    list-style: none;
    justify-content: center;
    @media (max-width:420px) {
      justify-content: end;
    }
    li {
      color: white;
      font-size: 20px;
    }
  }
  &__chat {
        align-items: baseline;
@media (max-width:420px) {
 
      width: 60%;
    }
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