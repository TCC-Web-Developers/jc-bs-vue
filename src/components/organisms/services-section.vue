<script setup>
import { ref } from "vue";
import BaseCard from "@/components/base-card.vue";

const services = ref([
  {
    id: 0,
    title: "Product Design",
  },
  {
    id: 1,
    title: "Cinematography",
  },
  {
    id: 2,
    title: "Web Design",
  },
]);
</script>

<template>
  <section class="d-flex align-items-center">
    <div class="container">
      <div class="row text-center pb-5">
        <h1 class="display-6 fw-light text-light">Services</h1>
      </div>
      <ul class="row">
        <li
          v-for="service in services"
          :key="service.id"
          class="col d-flex justify-content-center m-3"
        >
          <BaseCard :service="service" />
        </li>
      </ul>
    </div>
  </section>
</template>

<style lang="scss" scoped>
section {
  width: 100%;
  min-height: 100vh;
}
</style>
