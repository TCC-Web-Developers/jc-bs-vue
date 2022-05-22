<script setup>
const props = defineProps(["url", "style"]);
</script>

<template>
  <RouterLink class="base-link" :class="style" :to="url">
    <slot></slot>
  </RouterLink>
</template>

<style lang="scss" scoped>
.base-link {
  text-decoration: none;
}
</style>
