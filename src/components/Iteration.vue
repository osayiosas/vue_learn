<script setup>
import { ref } from "vue";

let peoples = ref(["james", "osayi", "Jaon"]);

const books = ref([
  {
    id: 1,
    title: "Book 1",
    author: "John Doe",
    gener: 'fication',
    publication: 2021,
  },

    {
        id: 2,
        title: "Book 2",
        author: "Osayi Idiahe",
        gener: 'poetry',
        publication: 1960,
    },
     {
        id: 3,
        title: "Book 3",
        author: "Joan Idiahe",
        gener: 'Drama',
        publication: 1960,
    },

     {
        id: 4,
        title: "Book 4",
        author: "Ernest Idiahe",
        gener: 'Dystopians',
        publication: 1930,
    },
     {
        id: 5,
        title: "Book 5",
        author: "johnson Idiahe",
        gener: 'poetry',
        publication: 1945,
    },
      
]);
</script>

<template>
  <p v-for="(person, index) in peoples" :key="index">
    {{ person }}
  </p>

  <ul v-for="({id, title, gener,author, publication}, index) in books" :key="index">
   <li>ID:{{ id }}</li>
    <li>Author:{{ author }}</li>
    <li>Title:{{ title }}</li>
    <li>Gener:{{ gener }}</li>
    <li>Publication Year:{{ publication }}</li>

  </ul>
</template>
