<script setup>
import { ref } from "vue";
import BaseLink from "@/components/atoms/base-link.vue";

const links = ref([
  {
    id: 0,
    name: "home",
    url: "/",
  },
  {
    id: 1,
    name: "service",
    url: "/service",
  },
  {
    id: 3,
    name: "about",
    url: "/about",
  },
]);
</script>

<template>
  <ul>
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
