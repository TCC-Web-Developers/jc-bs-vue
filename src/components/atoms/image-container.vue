<script setup>
const props = defineProps(["img"]);
</script>

<template>
  <img :src="img" alt="" />
</template>

<style lang="scss" scoped>
img {
  width: 50%;
}
</style>
