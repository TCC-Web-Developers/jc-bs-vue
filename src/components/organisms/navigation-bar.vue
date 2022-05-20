<script setup>
import TitleLogo from "@/components/atoms/title-logo.vue";
import NavigationLinks from "@/components/molecules/navigation-links.vue";
</script>

<template>
  <nav class="navbar bg-secondary position-fixed w-100 py-0">
    <div class="container">
      <TitleLogo>JC DESIGNS</TitleLogo>
      <NavigationLinks />
    </div>
  </nav>
</template>

<style lang="scss" scoped>
nav {
  z-index: 50;
  height: 10vh;
}
</style>
