<template>
  <div class="d-flex padding-listItem border-bottom border-color-gray w-60">
    <img :src="listItem.url" width="60" height="60" alt="">
    <div class="d-flex">
      <div class="pl-1 w-60">
        <div class="font-bold font-17">{{ listItem.courseName }}</div>
        <div class="d-flex pt-1">
          <button class="bg-yellow border-none" v-if="listItem.badge">{{ listItem.badge }}</button>
          <span class="color-hours pl-1 font-bold total-hour d-flex align-items-center">{{ listItem.hours }} total
            hours</span>
          <span class="pl-1">Updated {{ listItem.updatedDate }}</span>
        </div>
      </div>

      <div class="d-flex pl-5">
        <span class="mt-2 text-yellow1">{{ listItem.star }}</span>
        <img src="/img/star-filled.png" class="star-icon pr-3" alt="">
        <div class="d-flex">
          <svg class="svg-icon"
            style="width: 17px; height: 1.2rem; vertical-align: middle; fill: currentcolor; overflow: hidden;"
            viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg">
            <path
              d="M512 597.994667q108.010667 0 225.002667 46.997333t116.992 123.008l0 85.994667-684.010667 0 0-85.994667q0-76.010667 116.992-123.008t225.002667-46.997333zM512 512q-69.994667 0-120-50.005333t-50.005333-120 50.005333-121.002667 120-51.008 120 51.008 50.005333 121.002667-50.005333 120-120 50.005333z" />
          </svg>
          <span class="mt-2">{{ listItem.enteredNumber }}</span>
          <img src="/img/pound-icon.png" class="pound-icon" alt="">
          <span class="mt-2">{{ listItem.price }}</span>
          <button class="border-half-radius d-flex align-items-center heart-button pointer">
            <img src="/img/heart-icon.png" alt="">
          </button>
        </div>
      </div>
    </div>
  </div>


</template>

<style lang="postcss">
.border-half-radius {
  border-radius: 50%;
}

.w-75 {
  width: 75%;
}

.font-17 {
  font-size: 17px;
  line-height: 19px;
}

.pound-icon {
  width: 15px;
  height: 12px;
  margin-top: 3px;
  padding-left: 8px;
}

.padding-listItem {
  padding: 1.6rem 0;
}

.border-color-gray {
  border-color: #d1d7dc;
}

.border-bottom {
  border-bottom: 1px solid #d1d7dc;
}

.color-hours {
  color: #1e6055;
}

html {
  font-family: udemy sans, sf pro text, -apple-system, BlinkMacSystemFont, Roboto, segoe ui, Helvetica, Arial, sans-serif, apple color emoji, segoe ui emoji, segoe ui symbol;
}

.pr-3 {
  padding-right: 15px;
}

.mt-2 {
  margin-top: -2px;
}

.total-hour::after {
  content: '\25CF';
  font-size: 6px;
  margin-top: 2px;
  margin-left: 4px;
}

.heart-button {
  height: 34px;
  margin-left: 8px;
}

.text-yellow1 {
  color: #b4690e;
}
</style>

<script lang="ts">

export default {
  name: 'list-card',
  props: ['listItem'],
}

</script>