<script setup>
const props = defineProps(["img"]);
</script>

<template>
  <img
    :src="img"
    class="card-img img-fluid rounded-start"
    alt="product designing"
  />
</template>

<style lang="scss" scoped>
.card-img {
  display: block;
  width: 100%;
  height: 100%;
  object-fit: cover;
}
</style>
