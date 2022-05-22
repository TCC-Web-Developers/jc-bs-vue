<script setup>
const props = defineProps(["service"]);
</script>

<template>
  <div class="service-item">
    <div
      class="service-header d-flex align-items-center bg-secondary py-3 px-4 rounded"
    >
      <BaseRoundedIcon :size="'3rem'" :color="'primary'">
        <slot name="service-icon"></slot>
      </BaseRoundedIcon>
      <h2 class="display-6 fw-bold text-primary-text-light ms-4">
        {{ service.name }}
      </h2>
    </div>
    <div class="sevice-content py-5">
      <h3 class="fw-bold w-100 w-md-50 mb-3">
        Agency is a business you hire to outsource your digital marketing
        efforts
      </h3>
      <p class="lead w-100 w-md-50">
        Business you hire to outsource your digital marketing efforts, instead
        of handling in-house. They can provide your business with a variety of
        digital solutions to promote your product or service online and help
        you.
      </p>
    </div>
    <div class="service-features">
      <ul class="d-flex flex-column gap-3 p-0">
        <li class="feature d-flex align-items-center">
          <BaseRoundedIcon :size="'2rem'" :color="'accent'">
            <i
              class="bi bi-check-lg text-primary-text-light"
              style="font-size: 1rem"
            ></i>
          </BaseRoundedIcon>
          <div class="ms-3 fw-bold">Web Development</div>
        </li>
        <li class="feature d-flex align-items-center">
          <BaseRoundedIcon :size="'2rem'" :color="'accent'">
            <i
              class="bi bi-check-lg text-primary-text-light"
              style="font-size: 1rem"
            ></i>
          </BaseRoundedIcon>
          <div class="ms-3 fw-bold">Brand Strategy</div>
        </li>
        <li class="feature d-flex align-items-center">
          <BaseRoundedIcon :size="'2rem'" :color="'accent'">
            <i
              class="bi bi-check-lg text-primary-text-light"
              style="font-size: 1rem"
            ></i>
          </BaseRoundedIcon>
          <div class="ms-3 fw-bold">Art Direction</div>
        </li>
      </ul>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.service-item {
  margin-bottom: 6rem;
}
</style>
