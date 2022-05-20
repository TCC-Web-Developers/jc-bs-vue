<script setup>
import cardImg from "@/assets/images/card-img.png";
const props = defineProps(["service"]);
</script>

<template>
  <div class="card" style="width: 18rem">
    <div
      class="card-img-container d-flex justify-content-center align-items-center"
    >
      <img :src="cardImg" class="card-img" alt="..." />
    </div>
    <div class="card-body text-center">
      <h2 class="card-title">{{ service.title }}</h2>
      <p class="card-text pb-3">
        Some quick example text to build on the card title and make up the bulk
        of the card's content.
      </p>
      <a href="#" class="btn btn-primary text-light">Learn More</a>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.card {
  border-radius: 10px;

  .card-img-container {
    height: 10rem;

    .card-img {
      width: 50%;
      object-fit: content;
    }
  }
}
</style>
