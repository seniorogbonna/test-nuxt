<template>
  <div>
    <div class="d-flex border-top">
      <img :src="reviewData.url" width="30px" height="30px" alt="">
      <div class="flex-full">
        <p class="w-half">{{ reviewData.instructorName }}</p>
        <div class="d-flex">
          <img src="/img/star-filled.png" v-for="(star, i) in reviewData.rating" alt="">
          <div class="flex-full">{{ reviewData.time }}</div>
        </div>
      </div>
      <img src="/img/more-icon.png" alt="">
    </div>
    <div>
      {{ reviewData.description }}
    </div>
    <div class="d-flex w-half">
      <span>Helpful?</span>
      <img src="/img/thumbs-up.png" alt="">
      <img src="/img/thumbs-down.png" alt="">
    </div>
  </div>

</template>

<style lang="postcss">
.border-top {
  border-top: 1px solid #d1d7dc;
}
</style>

<script lang="ts">

export default {
  name: 'review-data',
  props: ['reviewData'],
}
</script>