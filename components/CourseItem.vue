<template>
  <div @click="openAccordion(textExpanded)" class="d-flex w-60 accordion-item-section pointer">
    <div v-if="textExpanded">
      <svg fill="#5624d0" height="14px" width="14px" version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg"
        xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 330 330" xml:space="preserve"
        style="margin-left: 4px; padding: 10px;">
        <path id="XMLID_224_"
          d="M325.606,229.393l-150.004-150C172.79,76.58,168.974,75,164.996,75c-3.979,0-7.794,1.581-10.607,4.394
	l-149.996,150c-5.858,5.858-5.858,15.355,0,21.213c5.857,5.857,15.355,5.858,21.213,0l139.39-139.393l139.397,139.393
	C307.322,253.536,311.161,255,315,255c3.839,0,7.678-1.464,10.607-4.394C331.464,244.748,331.464,235.251,325.606,229.393z" />
      </svg>

    </div>
    <div v-if="!textExpanded">
      <svg fill="#5624d0" height="14px" width="14px" version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg"
        xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 330 330" xml:space="preserve"
        style="margin-left: 4px; padding: 10px;">
        <path id="XMLID_225_" d="M325.607,79.393c-5.857-5.857-15.355-5.858-21.213,0.001l-139.39,139.393L25.607,79.393
	c-5.857-5.857-15.355-5.858-21.213,0.001c-5.858,5.858-5.858,15.355,0,21.213l150.004,150c2.813,2.813,6.628,4.393,10.606,4.393
	s7.794-1.581,10.606-4.394l149.996-150C331.465,94.749,331.465,85.251,325.607,79.393z" />
      </svg>
    </div>

    <div class="flex-full item-title font-bold">{{ courseItem.title }}</div>
    <div class="d-flex">
      <div class="text-sections d-flex align-items-center">{{ courseItem.lectures }} lectures</div>
      <div class="pl-1 d-flex align-items-center pr-29">{{ courseItem.time }}min</div>
    </div>
  </div>
  <div v-if="textExpanded">

    <div class="d-flex accordion-item-div w-60" v-for="(course, i) in courseItem.lectureDetail">
      <img src="/img/play-icon.png" class="play-icon" alt="">
      <div class="accordion-item-title">{{ course.title }}</div>
      <div class="accordion-item-time">{{ course.time }}</div>
    </div>
  </div>
</template>

<script lang="ts" setup>
import { defineComponent, PropType, ref } from 'vue';
import { defineProps, reactive } from "vue";
const textExpanded = ref<boolean>(false);
defineProps<{
  courseItem: {
    title: string,
    lectures: string,
    time: string,
    expanded: boolean,
    lectureDetail: {
      title: string,
      time: string,
    }[],
  }
}>();



function openAccordion(flag: boolean) {
  // console.log(courseItem.expanded);
  textExpanded.value = !flag;
}

</script>

<style lang="postcss">
.accordion-item-section {
  padding: 10px 20px;
  border: 1px solid #d1d7dc;
}

.item-title {
  font-size: 22px;
  padding-left: 24px;
}

.accordion-item-div {
  padding: 12px;
}

.play-icon {
  padding-left: 18px;
}

.accordion-item-title {
  padding-left: 25px;
  display: flex;
  align-items: center;
  flex: 1;
}

.accordion-item-time {
  padding-right: 20px;
}

.pr-29 {
  padding-right: 29px;
}
</style>