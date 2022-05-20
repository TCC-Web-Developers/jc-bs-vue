<script setup>
import NavigationBar from "@/components/organisms/navigation-bar.vue";
import HeroSection from "@/components/organisms/hero-section.vue";
import ClientsList from "@/components/organisms/clients-list.vue";
import ServicesSection from "@/components/organisms/services-section.vue";
</script>

<template>
  <main class="homepage bg-primary">
    <NavigationBar />
    <HeroSection />
    <ClientsList />
    <ServicesSection />
  </main>
  <!-- <RouterView /> -->
</template>

<style lang="scss">
@import "@/assets/base.css";
@import "@/assets/scss/custom.scss";
.homepage {
  width: 100%;
}
</style>
