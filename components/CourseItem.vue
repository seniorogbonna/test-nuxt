<template>
  <div class="d-flex w-60 accordion-item-section pointer">
    <svg fill="#5624d0" height="14px" width="14px" version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg"
      xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 330 330" xml:space="preserve"
      style="margin-left: 4px; padding: 10px;">
      <path id="XMLID_225_" d="M325.607,79.393c-5.857-5.857-15.355-5.858-21.213,0.001l-139.39,139.393L25.607,79.393
	c-5.857-5.857-15.355-5.858-21.213,0.001c-5.858,5.858-5.858,15.355,0,21.213l150.004,150c2.813,2.813,6.628,4.393,10.606,4.393
	s7.794-1.581,10.606-4.394l149.996-150C331.465,94.749,331.465,85.251,325.607,79.393z" />
    </svg>
    <div class="flex-full item-title">{{ courseItem.title }}</div>
    <div class="d-flex">
      <div class="text-sections d-flex align-items-center">{{ courseItem.lectures }} lectures</div>
      <div class="pl-1 d-flex align-items-center">{{ courseItem.time }}min</div>
    </div>
  </div>
  <div v-if="courseItem.expanded">
    <div class="d-flex" v-for="(course, i) in courseItem.lectureDetail">
      <img src="/img/play-icon.png" alt="">
      <div>{{ course.title }}</div>
      <div>{{ course.time }}</div>
    </div>
  </div>
</template>

<script lang="ts">

export default {
  name: 'course-item',
  props: ['courseItem'],
}

</script>

<style lang="postcss">
.accordion-item-section {
  padding: 10px 20px;
  border: 1px solid #d1d7dc;
}

.item-title {
  font-size: 22px;
  padding-left: 10px;
}
</style>