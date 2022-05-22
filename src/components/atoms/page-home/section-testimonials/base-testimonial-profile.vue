<template>
  <div class="testimonial-profile d-flex align-items-center pb-4 gap-3">
    <div class="testimonial-avatar mt-2">
      <slot name="testimonial-avatar"></slot>
    </div>
    <div class="testimonial-profile-info">
      <slot name="testimonial-name"></slot>
      <slot name="testimonial-work"></slot>
    </div>
  </div>
</template>
