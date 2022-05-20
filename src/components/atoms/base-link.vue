<script setup>
import { RouterLink } from "vue-router";

const props = defineProps(["metadata"]);
</script>

<template>
  <RouterLink class="link px-3 py-2" :to="metadata.url">
    {{ metadata.name }}
  </RouterLink>
</template>

<style lang="scss" scoped>
.link {
  text-decoration: none;
  text-transform: capitalize;
  color: #5662ea;

  &:hover {
    background-color: #4bd7f2;
    color: #ffffff;
    border-radius: 5px;
  }
}
</style>
