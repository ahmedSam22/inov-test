<template>
  <section class="container">
    <div class="header col-md-12">
      <h3 class="text-md-center text-bolder">التطبيقات المميزة</h3>
      <p class="text-md-center text-bold">
        تطبيقات تقدم حلول وخدمات مميزة نوصي بتجربتها
      </p>
    </div>

    <div class="card--container d-flex mt-5 row">
      <div
        class="card--container__card col-3"
        v-for="(card, index) of cards"
        :key="index"
      >
        <div class="card--container__card__header">
          <img :src="card.src" alt="" srcset="" width="44" height="44" />
          <div class="me-2">
            <span class="card--container__card__header__name">{{
              card.name
            }}</span>
            <span class="card--container__card__header__rate">
              <i class="fa-solid fa-star me-4"></i> {{ card.rate }}
            </span>
            <span class="card--container__card__header__developer">
              تطوير : <span class="text-muted">{{ card.developer }}</span>
            </span>
            <div class="card--container__card__header__title mt-2">
              <p class="m-0">
                {{ card.title }}
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
    <button class="btn btn-custom">
      جميع التطبيقات
      <i class="fa-solid fa-angle-left pe-2"></i>
    </button>
  </section>
</template>
<script>
export default {
  data() {
    return {
      cards: [
        {
          src: "https://icebreakerquestions.info/random-questions.jpg",
          name: "قمرة",
          rate: 5,
          developer: "عمر برهوم",
          title:
            "نظام الولاء الأمثل الذي يمكنك من رفع مبيعاتك نظام الولاء الأمثل الذي يمكنك من رفع مبيعاتك ",
        },
        {
          src: "https://icebreakerquestions.info/random-questions.jpg",
          name: "قمرة",
          rate: 5,
          developer: "عمر برهوم",
          title:
            "نظام الولاء الأمثل الذي يمكنك من رفع مبيعاتك نظام الولاء الأمثل الذي يمكنك من رفع مبيعاتك ",
        },
        {
          src: "https://icebreakerquestions.info/random-questions.jpg",
          name: "قمرة",
          rate: 5,
          developer: "عمر برهوم",
          title:
            "نظام الولاء الأمثل الذي يمكنك من رفع مبيعاتك نظام الولاء الأمثل الذي يمكنك من رفع مبيعاتك ",
        },
        {
          src: "https://icebreakerquestions.info/random-questions.jpg",
          name: "قمرة",
          rate: 5,
          developer: "عمر برهوم",
          title:
            "نظام الولاء الأمثل الذي يمكنك من رفع مبيعاتك نظام الولاء الأمثل الذي يمكنك من رفع مبيعاتك ",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
.header {
  p {
    @media (max-width: 400px) {
      width: 60%;
    }
  }
}
.card--container {
  flex-wrap: wrap;
  @media (max-width: 1000px) {
    overflow-x: scroll;
  }
  &__card {
    background: #f7f7f7;
    border-radius: 10px;
    margin: 10px 13px;
    width: 295px;
    padding: 22px;
    flex: none;
    &__header {
      display: flex;
      img {
        border-radius: 10px;
      }
      &__name {
        color: #8d5da7;
      }
      &__rate {
        svg {
          color: #ffd12f;
        }
      }
      &__developer {
        display: block;
      }
      &__title {
        p {
          font-size: 14px;
          line-height: 24px;
        }
      }
    }
  }
}
.btn-custom {
  color: #ffd12f;
  display: block;
  margin: auto;
}
</style>