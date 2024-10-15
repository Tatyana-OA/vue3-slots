<script setup>
import BaseButton from "./components/BaseButton.vue";
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
