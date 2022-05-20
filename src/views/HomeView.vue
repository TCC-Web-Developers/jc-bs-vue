<script setup>
import HeroSection from "@/components/organisms/hero-section.vue";
import ClientsList from "@/components/organisms/clients-list.vue";
import ServicesSection from "@/components/organisms/services-section.vue";
</script>

<template>
  <main class="homepage">
    <HeroSection />
    <ClientsList />
    <ServicesSection />
  </main>
</template>

<style lang="scss" scoped>
.homepage {
  width: 100%;
}
</style>
