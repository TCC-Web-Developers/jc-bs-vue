<script setup>
import AboutImg from "@/assets/images/about-img.png";
</script>

<template>
  <main>
    <BasePageHeader>
      <template v-slot:page-header-name>
        <BasePageHeaderName>About</BasePageHeaderName>
      </template>
      <template v-slot:page-header-message>
        <BasePageHeaderMessage>
          Agency provides a full service range including technical skills,
          design, business understanding.</BasePageHeaderMessage
        >
      </template>
    </BasePageHeader>
    <section class="img">
      <div class="container d-flex justify-content-center">
        <div class="img-container py-5">
          <img :src="AboutImg" alt="" />
        </div>
      </div>
    </section>
    <section class="about-info py-5">
      <div class="container d-flex justify-content-center">
        <div class="about-content w-50 text-start">
          <h5 class="fw-bold text-accent">JAKE CHRIST STARK</h5>
          <h1 class="fw-bolder display-6">
            PROFESSIONAL WEB DEVELOPER & GRAPHIC DESIGNER
          </h1>
          <p class="lead mt-5">
            Ability to put themselves in the merchant's shoes. It is meant to
            partner on the long run, and work as an extension of the merchant's
            team.
            <br /><br />
            A digital agency is a business you hire to outsource your digital
            marketing efforts, instead of handling in-house. They can provide
            your business with a variety of digital solutions to promote your
            product or service online and help you.
          </p>
        </div>
      </div>
    </section>
    <section class="about-experience py-5">
      <div class="container d-flex justify-content-center">
        <div class="experiences d-flex border py-5" style="width: max-content">
          <div class="years-experience d-flex align-items-center gap-4 px-5">
            <BaseRoundedIcon :size="'6rem'" :color="'accent'">
              <i
                class="bi bi-briefcase-fill text-primary-text-light"
                style="font-size: 3rem"
              ></i>
            </BaseRoundedIcon>
            <div class="experince-data">
              <div class="experince-data-percent h1 fw-bold">42%</div>
              <div class="experince-data-name h6 text-muted fw-bold">
                Years of Experience
              </div>
            </div>
          </div>
          <div
            class="project-done d-flex align-items-center gap-4 px-5 border-start"
          >
            <BaseRoundedIcon :size="'6rem'" :color="'accent'">
              <i
                class="bi bi-check2-square text-primary-text-light"
                style="font-size: 3rem"
              ></i>
            </BaseRoundedIcon>
            <div class="experince-data">
              <div class="experince-data-count h1 fw-bold">73+</div>
              <div class="experince-data-name h6 text-muted fw-bold">
                Projects Done
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  </main>
</template>

<style lang="scss" scoped>
main {
  min-height: 200vh;
  width: 100%;

  header {
    height: 45vh;
  }
}
</style>
