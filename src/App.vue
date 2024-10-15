<script setup>
import BaseButton from "./components/BaseButton.vue";
import BlogLayout from "./components/BlogLayout.vue";
import IconCommunity from "./components/icons/IconCommunity.vue";
import IconEcosystem from "./components/icons/IconEcosystem.vue";
import Library from "./components/Library.vue";

const imageAttrs = {
  src: "https://images.pexels.com/photos/312418/pexels-photo-312418.jpeg?cs=srgb&dl=pexels-chevanon-312418.jpg&fm=jpg",
  alt: "COFFEEEEEEEEEEEE",
  width: "300px",
  height: "auto",
};
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
    <Library />
    <img v-bind="imageAttrs" />
    <img
      v-bind:src="imageAttrs.src"
      v-bind:alt="imageAttrs.alt"
      v-bind:height="imageAttrs.height"
      v-bind:width="imageAttrs.width"
    />
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
