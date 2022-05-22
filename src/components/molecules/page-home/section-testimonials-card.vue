<script setup>
const props = defineProps(["testimonial"]);
</script>

<template>
  <BaseTestimonial>
    <template v-slot:testimonial-ratings>
      <BaseTestimonialRatings>
        <BaseStarsContainer />
      </BaseTestimonialRatings>
    </template>
    <template v-slot:testimonial-feedback>
      <BaseTestimonialFeedback>{{ testimonial.text }}</BaseTestimonialFeedback>
    </template>
    <template v-slot:testimonial-profile>
      <BaseTestimonialProfile>
        <template v-slot:testimonial-avatar>
          <img
            :src="testimonial.avatar"
            alt="avatar"
            class="img-fluid"
            style="height: 50px"
          />
        </template>
        <template v-slot:testimonial-name>
          <BaseTestimonialProfileName>{{
            testimonial.name
          }}</BaseTestimonialProfileName>
        </template>
        <template v-slot:testimonial-work>
          <BaseTestimonialProfileWork>{{
            testimonial.work
          }}</BaseTestimonialProfileWork>
        </template>
      </BaseTestimonialProfile>
    </template>
  </BaseTestimonial>
</template>
