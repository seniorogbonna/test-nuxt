<template>
  <div>
    <div class="d-flex border-top pt-5">
      <img :src="reviewData.url" width="50px" height="50px" class="border-half-radius" alt="">
      <div class="flex-full pl-3">
        <div class="w-half">{{ reviewData.instructorName }}</div>
        <div class="d-flex">
          <img src="/img/star-filled.png" width="20px" height="20px" v-for="(star, i) in ratings" alt="">
          <div class="flex-full">{{ reviewData.time }}</div>
        </div>
      </div>
      <img src="/img/more-icon.png" width="20px" height="30px" alt="">
    </div>
    <div class="pt-3">
      {{ reviewData.description }}
    </div>
    <div class="d-flex w-half pt-5">
      <span class="text-lightblack">Helpful?</span>
      <img src="/img/thumbs-up.png" width="21px" height="21px" style="margin-top: 2px; margin-left: 10px;" alt="">
      <img src="/img/thumbs-down.png" width="27px" height="24px" style="margin-left: 10px;" alt="">
    </div>
  </div>

</template>

<style lang="postcss">
.border-top {
  border-top: 1px solid #d1d7dc;
}

.pt-3 {
  padding-top: 12px;
}
</style>

<script lang="ts">

const stars = [1, 2, 3, 4, 5];

export default {
  name: 'review-data',
  props: ['reviewData'],

  data() {
    return {
      ratings: stars,
    }
  }
}
</script>