<script setup>
const props = defineProps(["img"]);
</script>

<template>
  <img :src="img" alt="" class="w-50" />
</template>

<style lang="scss" scoped></style>
