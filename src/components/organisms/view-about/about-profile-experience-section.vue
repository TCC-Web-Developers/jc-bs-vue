<template>
  <section class="about-experience py-5">
    <div class="container d-flex justify-content-center">
      <div
        class="experiences d-flex border py-5 bg-light"
        style="width: max-content"
      >
        <div class="years-experience d-flex align-items-center gap-4 px-5">
          <BaseRoundedIcon :size="'5rem'" :color="'accent'">
            <i
              class="bi bi-briefcase-fill text-primary-text-light"
              style="font-size: 2.5rem"
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
          <BaseRoundedIcon :size="'5rem'" :color="'accent'">
            <i
              class="bi bi-check2-square text-primary-text-light"
              style="font-size: 2.5rem"
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
</template>
