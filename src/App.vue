<script setup>
import BaseButton from "./components/BaseButton.vue";
import BlogLayout from "./components/BlogLayout.vue";
import IconCommunity from "./components/icons/IconCommunity.vue";
import IconEcosystem from "./components/icons/IconEcosystem.vue";
</script>

<template>
  <header></header>

  <main>
    <BaseButton>
      <div class="flex-btn">
        <IconEcosystem />
        <h3>Button Text</h3>
        <IconCommunity />
      </div>
    </BaseButton>
    <BlogLayout>
      <template v-slot:header>
        <h1>My Page</h1>
      </template>
      <template v-slot:main>
        <p>My page content</p>
      </template>
      <template v-slot:sidebar>
        <ul>
          <li>Bullet 1</li>
          <li>Bullet 2</li>
        </ul>
      </template>
    </BlogLayout>
  </main>
</template>

<style>
.flex-btn {
  display: flex;
  flex-direction: row;
  gap: 10px;
  align-items: center;
}
</style>
