<script setup>
import { computed } from "vue";
import { RouterLink, useRouter } from "vue-router";

const router = useRouter();

const props = defineProps(["metadata"]);

const currentRoute = computed(() => {
  return router.currentRoute.value.fullPath;
});
</script>

<template>
  <RouterLink
    class="link px-3 py-2 h-100 d-flex align-items-center"
    :class="[metadata.url === currentRoute ? 'fw-bold' : 'fw-normal']"
    :to="metadata.url"
  >
    {{ metadata.name }}
    <div
      v-show="metadata.url === currentRoute"
      class="current-link-indicator bg-primary"
    ></div>
  </RouterLink>
</template>

<style lang="scss" scoped>
.link {
  text-decoration: none;
  text-transform: capitalize;
  color: #5662ea;
  position: relative;

  .current-link-indicator {
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;
    height: 0.4rem;
  }

  &:hover {
    backdrop-filter: contrast(0.9);
  }
}
</style>
