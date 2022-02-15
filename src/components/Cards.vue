<template>
<section class="container">
     <h3 class="text-center text-bolder">التطبيقات المميزة</h3>
      <p class="text-center text-bold">تطبيقات تقدم حلول وخدمات مميزة نوصي بتجربتها</p>

  <div class="card--container d-flex mt-5">
    <div
      class="card--container__card"
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
            تطوير :  <span class="text-muted">{{ card.developer }}</span> 
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
        }
      ],
    };
  },
};
</script>

<style scoped lang="scss">
.card--container {
  flex-wrap: nowrap;
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
</style>