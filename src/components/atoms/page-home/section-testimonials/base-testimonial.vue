<template>
  <div
    class="testimonial-container d-flex justify-content-center align-items-center py-3"
  >
    <div class="testimonial-content bg-light px-4 py-2 rounded-3 shadow-sm">
      <slot name="testimonial-ratings"></slot>
      <slot name="testimonial-feedback"></slot>
      <slot name="testimonial-profile"></slot>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.testimonial-container {
  width: 100%;

  .testimonial-content {
    width: 50%;
    height: 80%;
  }
}
</style>
