<template>
  <div class="book">
    <slot
      name="title"
      :bookTitle="bookTitle"
      :capitalizedTitle="computedUppercaseTitle"
    />
  </div>
</template>

<script setup>
import { computed } from "vue";
const bookTitle = "Hello, darkness, my old friend";
const computedUppercaseTitle = computed(() => bookTitle.toUpperCase());
</script>
