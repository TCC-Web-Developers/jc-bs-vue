<script setup>
import AdidasIcon from "@/components/atoms/icons/adidas-icon.vue";
import Apple from "@/components/atoms/icons/apple-icon.vue";
import Google from "@/components/atoms/icons/google-icon.vue";
import Intercom from "@/components/atoms/icons/intercom-icon.vue";
import Nike from "@/components/atoms/icons/nike-icon.vue";
import Samsung from "@/components/atoms/icons/samsung-icon.vue";
</script>

<template>
  <ul>
    <li>
      <AdidasIcon />
    </li>
    <li>
      <Apple />
    </li>
    <li>
      <Google />
    </li>
    <li>
      <Intercom />
    </li>
    <li>
      <Nike />
    </li>
    <li>
      <Samsung />
    </li>
  </ul>
</template>

<style lang="scss" scoped>
ul {
  list-style: none;
  padding: 0;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 4rem;
}
</style>
