<template>
  <h2>Students Also bought</h2>
  <ListCard v-for="(list, i) in listItems" :listItem="list" :key="i" />
</template>

<script lang="ts">
const listItemsData = [
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

export default {
  data() {
    return {
      listItems: listItemsData,
    }
  }
}
</script>