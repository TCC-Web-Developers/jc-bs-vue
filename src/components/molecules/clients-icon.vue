<script setup>
import AdidasIcon from "@/components/atoms/icons/adidas-icon.vue";
import Apple from "@/components/atoms/icons/apple-icon.vue";
import Google from "@/components/atoms/icons/google-icon.vue";
import Intercom from "@/components/atoms/icons/intercom-icon.vue";
import Nike from "@/components/atoms/icons/nike-icon.vue";
import Samsung from "@/components/atoms/icons/samsung-icon.vue";
</script>

<template>
  <ul class="row">
    <li
      class="col-6 col-sm-4 col-lg d-flex align-items-center justify-content-center py-4 py-lg-0"
    >
      <AdidasIcon />
    </li>
    <li
      class="col-6 col-sm-4 col-lg d-flex align-items-center justify-content-center py-4 py-lg-0"
    >
      <Apple />
    </li>
    <li
      class="col-6 col-sm-4 col-lg d-flex align-items-center justify-content-center py-4 py-lg-0"
    >
      <Google />
    </li>
    <li
      class="col-6 col-sm-4 col-lg d-flex align-items-center justify-content-center py-4 py-lg-0"
    >
      <Intercom />
    </li>
    <li
      class="col-6 col-sm-4 col-lg d-flex align-items-center justify-content-center py-4 py-lg-0"
    >
      <Nike />
    </li>
    <li
      class="col-6 col-sm-4 col-lg d-flex align-items-center justify-content-center py-4 py-lg-0"
    >
      <Samsung />
    </li>
  </ul>
</template>

<style lang="scss" scoped>
ul {
  list-style: none;
  padding: 0;
  width: 100%;
}
</style>
