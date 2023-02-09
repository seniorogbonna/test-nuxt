<template>
  <h2>Course Content</h2>
  <div class="d-flex w-60">
    <p class="text-sections pl-1">19 sections</p>
    <p class="text-lectures pl-1">126 lectures</p>
    <p class="pl-1">19h 3m total length</p>
    <p class="color-strongPurple justify-content-end flex-full pointer">Expand all sections</p>
  </div>
  <CourseItem v-for="(course, i) in courseItems" :courseItem="course" :key="i" />
</template>

<style lang="postcss">
.justify-content-end {
  display: flex;
  justify-content: flex-end;
}

.flex-full {
  flex: 1;
}


.text-sections::after,
.text-lectures::after {
  content: '\25CF';
  padding-left: 4px;
}
</style>

<script lang="ts" setup>
import { defineComponent, PropType, ref } from 'vue'
const courseItems = [
  {
    title: "Introduzione",
    lectures: "5",
    time: "37",
    expanded: false,
    lectureDetail: [
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      }
    ]
  },
  {
    title: "Introduzione",
    lectures: "5",
    time: "37",
    expanded: false,
    lectureDetail: [
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      }
    ]
  },
  {
    title: "Introduzione",
    lectures: "5",
    time: "37",
    expanded: false,
    lectureDetail: [
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      }
    ]
  },
  {
    title: "Introduzione",
    lectures: "5",
    time: "37",
    expanded: false,
    lectureDetail: [
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      }
    ]
  },
  {
    title: "Introduzione",
    lectures: "5",
    time: "37",
    expanded: false,
    lectureDetail: [
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      }
    ]
  },
  {
    title: "Introduzione",
    lectures: "5",
    time: "37",
    expanded: false,
    lectureDetail: [
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      }
    ]
  },
  {
    title: "Introduzione",
    lectures: "5",
    time: "37",
    expanded: false,
    lectureDetail: [
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      }
    ]
  },
  {
    title: "Introduzione",
    lectures: "5",
    time: "37",
    expanded: false,
    lectureDetail: [
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      }
    ]
  },
  {
    title: "Introduzione",
    lectures: "5",
    time: "37",
    expanded: false,
    lectureDetail: [
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      }
    ]
  },
  {
    title: "Introduzione",
    lectures: "5",
    time: "37",
    expanded: false,
    lectureDetail: [
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      }
    ]
  },
  {
    title: "Introduzione",
    lectures: "5",
    time: "37",
    expanded: false,
    lectureDetail: [
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      }
    ]
  },
  {
    title: "Introduzione",
    lectures: "5",
    time: "37",
    expanded: false,
    lectureDetail: [
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      },
      {
        title: "Differenze tra Mac e Win",
        time: "03:18"
      }
    ]
  },
];


</script>