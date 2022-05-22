<script setup>
const props = defineProps(["size", "color"]);
</script>

<template>
  <div
    class="icon-circle rounded-circle d-flex justify-content-center align-items-center"
    :class="[
      color === 'primary'
        ? 'bg-primary'
        : color === 'secondary'
        ? 'bg-secondary'
        : 'bg-accent',
    ]"
    :style="{ height: size }"
  >
    <slot></slot>
  </div>
</template>

<style lang="scss" scoped>
.icon-circle {
  aspect-ratio: 1/1;
}
</style>
