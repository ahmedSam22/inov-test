<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-md-6 col-8">
        <div class="content p-lg-5">
          <div class="content__text">
            <h1>كل ما تحتاجه لنمو متجرك فى مكان واحد</h1>
            <p>
              مميزات سوق تطبيقات زد تساعدك في سهولة وسرعة الاستفادة من خدمات
              وحلول سوق التطبيقات لنمو متجرك ومضاعفة أرباحك
            </p>
          </div>
          <div class="content__utilities">
            <ul>
              <li>
                <img src="../assets/mng.png" class="ms-lg-3 d-block" alt="" srcset="" />
                <p>
                  سهولة ادارة و تفعيل تطبيقاتك من  لوحة تحكم متجرك
                </p>
              </li>
              <li>
                <img src="../assets/cs.png" class="ms-lg-3" alt="" srcset="" />
                <p> دعم فني و تقني متكامل متوفر على مدار الساعة </p>
              </li>
              <li>
                <img src="../assets/price.png" class="ms-lg-3" alt="" srcset="" />
                <p>أسعار تنافسية مع تجربة مجانية وباقات اشتراك متنوعة </p>
              </li>
            </ul>
            <button class="btn content__utilities__btn-custom mb-3">
              تصفّح التطبيقات
              <i class="fa-solid fa-angle-left pe-2"></i>
            </button>
          </div>
        </div>
      </div>
      <div class="col-md-6  col-8">
        <div class="main">
          <div class="dot-pattern"></div>
          <div class="main__slider">
            <img src="../assets/logo.png" height="100" alt="" srcset="" />
            <div class="main__slider__layer"></div>
          </div>

          <div class="bg-circle"></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import url("../style/Global.scss");

.container-fluid {
  background: rgba(250, 250, 252, 0.93);
  .content {
    @media (max-width: 770px) {
      padding: 0;
    }
    padding: 20px;
    h1 {
      color: #8d5da7;
      font-weight: bold;
    }
    p {
      font-size: 24px;
      color: #000;
      line-height: 34px;
    }
    &__utilities {
      ul {
        list-style: none;
        padding: 0px;
        margin-top: 10px;
        li {
          margin-bottom: 20px;
          display: flex;
          align-items: end;
 @media (max-width: 770px) {
          align-items: center;
          }
          p {
            font-size: 18px;
            color: #000000;
            @media (max-width: 770px) {
            font-size: 14px;
          }
          }
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
      }
    }
  }
  .main {
    position: relative;
    padding: 20px;
    display: flex;
    justify-content: center;
    height: 556px;
    align-items: center;
    @media (max-width: 770px) {
      padding: 0;
      height: 350px;
    }
    &__slider {
      width: 846.89px;
      height: 441px;
      background: #8d5da7;
      border-radius: 40px;
      z-index: 1;
      overflow: hidden;
      position: relative;
      @media (max-width: 770px) {
        width: 450px;
        height: 349.29px;
      }
      img {
        position: absolute;
        top: calc(441px / 2) - 50px;
        left: calc(450px / 2 ) + 50px;
        opacity: 0.7;
        @media (max-width: 770px) {
          // display: none;
        }
      }
      &__layer {
        height: 100%;
        width: 100%;
        background: url("../assets/bg.jpg");
        background-size: cover;
      }
    }
  }
  .dot-pattern {
    position: absolute;
    left: -30px;
    top: 15px;
    @media (max-width: 1245px) {
      display: none;
    }
  }

  .bg-circle {
    position: absolute;
    right: -120px;
    bottom: -34px;
    @media (max-width: 1245px) {
      display: none;
    }
  }
}
</style>