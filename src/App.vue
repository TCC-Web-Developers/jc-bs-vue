<script setup>
import NavigationBar from "@/components/organisms/navigation-bar.vue";
</script>

<template>
  <NavigationBar />
  <RouterView />
</template>

<style lang="scss">
@import "@/assets/base.css";
@import "@/assets/scss/custom.scss";
.homepage {
  width: 100%;
}
</style>
