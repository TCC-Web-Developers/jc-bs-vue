<script setup>
import NavigationBar from "@/components/organisms/navigation-bar.vue";
</script>

<template>
  <main class="portfolio bg-primary w-100 pb-5">
    <NavigationBar />
    <div class="spacer"></div>
    <RouterView />
  </main>
</template>

<style lang="scss">
@import "@/assets/base.css";
@import "@/assets/scss/custom.scss";

.portfolio {
  min-height: 100vh;

  .spacer {
    height: 10vh;
  }
}
</style>
