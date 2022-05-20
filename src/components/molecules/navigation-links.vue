<script setup>
import { ref } from "vue";
import BaseLink from "@/components/atoms/base-link.vue";

const links = ref([
  {
    id: 0,
    name: "home",
    url: "/",
    isActive: true,
  },
  {
    id: 1,
    name: "service",
    url: "/service",
    isActive: false,
  },
  {
    id: 3,
    name: "about",
    url: "/about",
    isActive: false,
  },
]);
</script>

<template>
  <ul class="align-self-stretch">
    <li v-for="link in links" :key="link.id">
      <BaseLink :metadata="link" />
    </li>
  </ul>
</template>

<style lang="scss" scoped>
ul {
  list-style: none;
  padding: 0;
  display: flex;
}
</style>
