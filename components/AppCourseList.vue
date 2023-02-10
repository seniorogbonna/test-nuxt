<template>
  <h2>Students Also bought</h2>
  <ListCard v-for="(list, i) in listItemData" :listItem="list" :key="i" />
  <div>
    <button @click="showButton(expand)" class="w-60 show-button pointer">{{ expand? 'Show Less': 'Show More' }}</button>
  </div>

</template>

<style lang="postcss">
.show-button {
  width: 60%;
  font-size: 20px;
  padding-top: 12px;
  padding-bottom: 12px;
}
</style>

<script lang="ts" setup>
import { defineComponent, PropType, ref } from 'vue'
let listItemsData = [
  {
    url: "/img/image.jpg",
    courseName: "Adobo Photoshop CC -- Essentials Traiging Course",
    badge: "Bestseller",
    hours: "11",
    updatedDate: "4/2022",
    star: "4.7",
    enteredNumber: "11,456",
    price: "59.99",
  },
  {
    url: "/img/image.jpg",
    courseName: "Adobo Photoshop CC -- Essentials Traiging Course",
    badge: "Bestseller",
    hours: "11",
    updatedDate: "4/2022",
    star: "4.7",
    enteredNumber: "11,456",
    price: "59.99",
  },
  {
    url: "/img/image.jpg",
    courseName: "Adobo Photoshop CC -- Essentials Traiging Course",
    badge: "Bestseller",
    hours: "11",
    updatedDate: "4/2022",
    star: "4.7",
    enteredNumber: "11,456",
    price: "59.99",
  },
  {
    url: "/img/image.jpg",
    courseName: "Adobo Photoshop CC -- Essentials Traiging Course",
    badge: "Bestseller",
    hours: "11",
    updatedDate: "4/2022",
    star: "4.7",
    enteredNumber: "11,456",
    price: "59.99",
  },
  {
    url: "/img/image.jpg",
    courseName: "Adobo Photoshop CC -- Essentials Traiging Course",
    badge: "Bestseller",
    hours: "11",
    updatedDate: "4/2022",
    star: "4.7",
    enteredNumber: "11,456",
    price: "59.99",
  },
  {
    url: "/img/image.jpg",
    courseName: "Adobo Photoshop CC -- Essentials Traiging Course",
    badge: "Bestseller",
    hours: "11",
    updatedDate: "4/2022",
    star: "4.7",
    enteredNumber: "11,456",
    price: "59.99",
  },
  {
    url: "/img/image.jpg",
    courseName: "Adobo Photoshop CC -- Essentials Traiging Course",
    badge: "Bestseller",
    hours: "11",
    updatedDate: "4/2022",
    star: "4.7",
    enteredNumber: "11,456",
    price: "59.99",
  },
  {
    url: "/img/image.jpg",
    courseName: "Adobo Photoshop CC -- Essentials Traiging Course",
    badge: "Bestseller",
    hours: "11",
    updatedDate: "4/2022",
    star: "4.7",
    enteredNumber: "11,456",
    price: "59.99",
  },
  {
    url: "/img/image.jpg",
    courseName: "Adobo Photoshop CC -- Essentials Traiging Course",
    badge: "Bestseller",
    hours: "11",
    updatedDate: "4/2022",
    star: "4.7",
    enteredNumber: "11,456",
    price: "59.99",
  },
  {
    url: "/img/image.jpg",
    courseName: "Adobo Photoshop CC -- Essentials Traiging Course",
    badge: "Bestseller",
    hours: "11",
    updatedDate: "4/2022",
    star: "4.7",
    enteredNumber: "11,456",
    price: "59.99",
  },
  {
    url: "/img/image.jpg",
    courseName: "Adobo Photoshop CC -- Essentials Traiging Course",
    badge: "Bestseller",
    hours: "11",
    updatedDate: "4/2022",
    star: "4.7",
    enteredNumber: "11,456",
    price: "59.99",
  },
  {
    url: "/img/image.jpg",
    courseName: "Adobo Photoshop CC -- Essentials Traiging Course",
    badge: "Bestseller",
    hours: "11",
    updatedDate: "4/2022",
    star: "4.7",
    enteredNumber: "11,456",
    price: "59.99",
  },
];
// const temp = listItemsData.slice(0, 4);
const tempData = ref<{}[]>(listItemsData);
const listItemData = ref<{}[]>(listItemsData);
const expand = ref<boolean>(false);
listItemData.value = tempData.value.slice(0, 4);

function showButton(flag: boolean) {

  expand.value = !flag;
  if (!expand.value) {
    listItemData.value = tempData.value.slice(0, 4);
  } else {
    listItemData.value = tempData.value;
  }
}



</script>