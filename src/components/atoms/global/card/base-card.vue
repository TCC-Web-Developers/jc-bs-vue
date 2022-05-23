<script setup>
const props = defineProps(["color", "shadow", "hover", "rounded"]);
const colorTypes = ref([
  "secondary",
  "primary",
  "accent",
  "light",
  "transparent",
]);

const getCardColor = computed(() => {
  const type = colorTypes.value.find(type => type === props.color);
  return `bg-${type}`;
});

const shadowEnable = computed(() => {
  return props.shadow;
});

const hoverEnable = computed(() => {
  return props.hover ? "hover" : "";
});

const roundedEnable = computed(() => {
  return props.rounded;
});
</script>

<template>
  <div :class="[getCardColor, shadowEnable, hoverEnable]">
    <slot name="card-head"></slot>
    <slot name="card-body"></slot>
    <slot name="card-foot"></slot>
  </div>
</template>

<style lang="scss" scoped>
.base-card {
  transition: 0.2s all linear;
}

.hover {
  &:hover {
    transform: scale(1.04);
    box-shadow: 0 20px 25px -5px rgb(0 0 0 / 0.1),
      0 8px 10px -6px rgb(0 0 0 / 0.1);
  }
}

.shadow {
  box-shadow: 0 4px 6px -1px rgb(0 0 0 / 0), 0 2px 4px -2px rgb(0 0 0 / 0);
}
</style>
