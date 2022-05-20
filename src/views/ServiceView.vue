<script setup>
import ServiceContent from "@/components/organisms/service-page/service-content.vue";
</script>

<template>
  <main class="service-page w-100">
    <div class="container">
      <div class="title py-5">
        <h1 class="display-6 text-light">SERVICES</h1>
      </div>
      <div class="services">
        <ServiceContent />
      </div>
    </div>
  </main>
</template>

<style lang="scss" scoped>
.card-img {
  display: block;
  width: 100%;
  height: 100%;
  object-fit: cover;
}
</style>
