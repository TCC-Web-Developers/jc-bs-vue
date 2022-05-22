<script setup>
import AboutImg from "@/assets/images/about-img.png";
</script>

<template>
  <section class="img">
    <div class="container d-flex justify-content-center">
      <div class="img-container py-5">
        <img :src="AboutImg" alt="" class="img-fluid" />
      </div>
    </div>
  </section>
</template>
