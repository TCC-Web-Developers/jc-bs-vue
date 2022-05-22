<script setup>
import { Tooltip } from "bootstrap";
import Logo1Img from "@/assets/images/logo1-img.png";
import Logo2Img from "@/assets/images/logo2-img.png";
import Logo3Img from "@/assets/images/logo3-img.png";
import Logo4Img from "@/assets/images/logo4-img.png";
import Logo5Img from "@/assets/images/logo5-img.png";

onMounted(() => {
  var tooltipTriggerList = [].slice.call(
    document.querySelectorAll('[data-bs-toggle="tooltip"]')
  );
  var tooltipList = tooltipTriggerList.map(function (tooltipTriggerEl) {
    return new Tooltip(tooltipTriggerEl);
  });
});
</script>

<template>
  <section class="clients-icon-section">
    <div class="container">
      <div
        class="company-icons d-flex align-items-center justify-content-center flex-wrap gap-5"
      >
        <div
          class="icon-container"
          data-bs-toggle="tooltip"
          data-bs-placement="top"
          title="Wired"
        >
          <img :src="Logo1Img" alt="icon" class="img-fluid" />
        </div>
        <div
          class="icon-container"
          data-bs-toggle="tooltip"
          data-bs-placement="top"
          title="Forbes"
        >
          <img :src="Logo2Img" alt="icon" class="img-fluid" />
        </div>
        <div
          class="icon-container"
          data-bs-toggle="tooltip"
          data-bs-placement="top"
          title="Bloomberg"
        >
          <img :src="Logo3Img" alt="icon" class="img-fluid" />
        </div>
        <div
          class="icon-container"
          data-bs-toggle="tooltip"
          data-bs-placement="top"
          title="Airbnb"
        >
          <img :src="Logo4Img" alt="icon" class="img-fluid" />
        </div>
        <div
          class="icon-container"
          data-bs-toggle="tooltip"
          data-bs-placement="top"
          title="Adobe"
        >
          <img :src="Logo5Img" alt="icon" class="img-fluid" />
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.company-icons {
  padding: 6rem 0;

  .icon-container {
    img {
      opacity: 0.4;
    }
  }
}
</style>
