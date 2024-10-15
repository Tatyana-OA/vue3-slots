<template>
  <div class="book">
    <slot name="title" :bookTitle="bookTitle" />
  </div>
</template>

<script setup>
const bookTitle = "Hello, darkness, my old friend";
</script>
