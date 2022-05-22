<script setup>
const router = useRouter();
const props = defineProps(["url"]);

const currentRoute = computed(() => {
  return router.currentRoute.value.fullPath;
});
</script>

<template>
  <li class="px-3 h-100">
    <BaseLink
      :url="url"
      :style="'h-100 d-flex align-items-center text-primary-text-light'"
    >
      <slot></slot>
    </BaseLink>
    <div
      v-show="currentRoute === url"
      class="current-route-indicator bg-primary"
    ></div>
  </li>
</template>

<style lang="scss" scoped>
li {
  position: relative;

  &:hover {
    backdrop-filter: contrast(1.3);
  }

  .current-route-indicator {
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;
    height: 0.3rem;
  }
}
</style>
