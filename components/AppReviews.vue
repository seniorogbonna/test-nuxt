<template>
  <h1 class="d-flex align-items-center">
    <img src="/img/star-filled.png" width="30px" height="30px" alt="">
    <span class="review-rating-text pr-3">4.6 course rating</span>
    5K ratings
  </h1>

  <div class="d-flex flex-wrap justify-content-between">
    <AppReviewItem class="w-46 review-item-section" v-for="(reviewItem, i) in reviews" :reviewData=reviewItem
      :key="i" />
  </div>

</template>

<style lang="postcss">
.review-rating-text::after {
  padding-left: 12px;
  content: '\25CF';
  color: #6a6f73;
}

.justify-content-between {
  justify-content: space-between;
}

.justify-content-around {
  justify-content: space-around;
}

.flex-wrap {
  flex-wrap: wrap;
}

.w-46 {
  width: 46%;
}

.review-item-section {
  padding-left: 10px;
  padding-bottom: 10px;
}
</style>

<script lang="ts">
const reviews = [
  {
    url: "/img/image.jpg",
    instructorName: "Lorenzo G",
    ratings: 5,
    time: "3 weeks ago",
    description: "Felice e soddisfatta del corso Adobe Photoshop di Alberto Comper. Metodo di insegnamento semplice ed efficace.Insegnante gentile e disponibile.Super consigliato!"
  },
  {
    url: "/img/image.jpg",
    instructorName: "Lorenzo G",
    ratings: 5,
    time: "3 weeks ago",
    description: "Felice e soddisfatta del corso Adobe Photoshop di Alberto Comper. Metodo di insegnamento semplice ed efficace.Insegnante gentile e disponibile.Super consigliato!"
  },
  {
    url: "/img/image.jpg",
    instructorName: "Lorenzo G",
    ratings: 5,
    time: "3 weeks ago",
    description: "Felice e soddisfatta del corso Adobe Photoshop di Alberto Comper. Metodo di insegnamento semplice ed efficace.Insegnante gentile e disponibile.Super consigliato!"
  },
  {
    url: "/img/image.jpg",
    instructorName: "Lorenzo G",
    ratings: 5,
    time: "3 weeks ago",
    description: "Felice e soddisfatta del corso Adobe Photoshop di Alberto Comper. Metodo di insegnamento semplice ed efficace.Insegnante gentile e disponibile.Super consigliato!"
  },
  {
    url: "/img/image.jpg",
    instructorName: "Lorenzo G",
    ratings: 5,
    time: "3 weeks ago",
    description: "Felice e soddisfatta del corso Adobe Photoshop di Alberto Comper. Metodo di insegnamento semplice ed efficace.Insegnante gentile e disponibile.Super consigliato!"
  },
];

export default {
  data() {
    return {
      reviews: reviews
    }
  }
}

</script>