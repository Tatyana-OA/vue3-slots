<template>
  <Book>
    <template v-slot:title="slotProps">
      <h1>{{ slotProps.bookTitle }}</h1>
    </template>
  </Book>
</template>

<script setup>
import Book from "./Book.vue";
</script>
