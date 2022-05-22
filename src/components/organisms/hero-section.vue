<script setup>
import HeroSectionImg from "@/assets/images/herosection-img.png";
</script>

<template>
  <section class="hero-section bg-secondary">
    <div class="container">
      <div class="row">
        <div
          class="left-content col-12 col-md-6 text-center text-md-end d-flex align-items-center"
        >
          <div class="left-content text-primary-text-light pt-5 pt-md-0">
            <header class="herosection-text">
              <h6 class="text-accent fw-bold">
                Web Design Expert | Product Designer
              </h6>
              <h1 class="display-5 fw-bolder">
                JC WEB DESIGN <br />
                STUDIO
              </h1>
              <p class="lead">
                Lorem ipsum dolor sit amet consectetur adipisicing elit.
                Cupiditate molestiae at odio.
              </p>
            </header>
            <div
              class="btns d-flex justify-content-center justify-content-md-end mt-4"
            >
              <button class="btn btn-accent text-primary-text-light">
                Explore Now
              </button>
              <button class="btn btn-outline-primary btn-transparent ms-3">
                Contact
              </button>
            </div>
          </div>
        </div>

        <div class="right-content col-12 col-md-6 d-flex align-items-center">
          <img :src="HeroSectionImg" alt="herosection" class="img-fluid" />
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.hero-section {
  .container {
    padding-bottom: 5rem;
  }
}
</style>
