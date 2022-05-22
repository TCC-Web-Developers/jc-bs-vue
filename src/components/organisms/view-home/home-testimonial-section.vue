<script setup>
import User1Img from "@/assets/images/user1-img.png";
import User2Img from "@/assets/images/user2-img.png";
import User3Img from "@/assets/images/user3-img.png";
import User4Img from "@/assets/images/user4-img.png";
import { Carousel } from "bootstrap";

const carousel = ref(null);

const testimonials = ref([
  {
    id: 1,
    avatar: User1Img,
    name: "Marry Thompson",
    work: "Starbucks",
    text: "A digital agency is a business you hire to outsource your digital marketing efforts, instead of handling in-house. They can provide your business with a variety of digital solutions to promote your product or service online and help you.",
  },
  {
    id: 2,
    avatar: User2Img,
    name: "John Doe",
    work: "Starbucks",
    text: "A digital agency is a business you hire to outsource your digital marketing efforts, instead of handling in-house. They can provide your business with a variety of digital solutions to promote your product or service online and help you.",
  },
  {
    id: 3,
    avatar: User3Img,
    name: "Francis Jobs",
    work: "Starbucks",
    text: "A digital agency is a business you hire to outsource your digital marketing efforts, instead of handling in-house. They can provide your business with a variety of digital solutions to promote your product or service online and help you.",
  },
  {
    id: 4,
    avatar: User4Img,
    name: "Mark bezos",
    work: "Starbucks",
    text: "A digital agency is a business you hire to outsource your digital marketing efforts, instead of handling in-house. They can provide your business with a variety of digital solutions to promote your product or service online and help you.",
  },
]);

onMounted(() => {
  var myCarousel = document.querySelector("#myCarousel");
  carousel.value = new Carousel(myCarousel, {
    interval: 2000,
    wrap: false,
  });
});
</script>

<template>
  <section class="testimonials-section">
    <div class="container">
      <BaseSectionHeader>
        <template v-slot:section-name>TESTIMONIALS </template>
        <template v-slot:section-message>
          <h1 class="display-5 section-message text-secondary">
            WHAT MY CLIENT SAYING
          </h1>
        </template>
      </BaseSectionHeader>
      <div id="myCarousel" class="carousel slide" data-bs-ride="carousel">
        <div class="carousel-inner">
          <div class="carousel-item active">
            <SectionTestimonialsCard :testimonial="testimonials[0]" />
          </div>
          <div class="carousel-item">
            <SectionTestimonialsCard :testimonial="testimonials[1]" />
          </div>
          <div class="carousel-item">
            <SectionTestimonialsCard :testimonial="testimonials[2]" />
          </div>
          <div class="carousel-item">
            <SectionTestimonialsCard :testimonial="testimonials[3]" />
          </div>
        </div>
        <button
          @click="carousel.prev()"
          class="carousel-control-prev bg-secondary rounded"
          type="button"
          data-bs-target="#carouselExampleControls"
          data-bs-slide="prev"
        >
          <span class="carousel-control-prev-icon" aria-hidden="true"></span>
          <span class="visually-hidden">Previous</span>
        </button>
        <button
          @click="carousel.next()"
          class="carousel-control-next bg-secondary rounded"
          type="button"
          data-bs-target="#carouselExampleControls"
          data-bs-slide="next"
        >
          <span class="carousel-control-next-icon" aria-hidden="true"></span>
          <span class="visually-hidden">Next</span>
        </button>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.container {
  padding-bottom: 6rem;
  .testimonial-container {
    width: 100%;

    .testimonial-content {
      width: 50%;
      height: 80%;
    }
  }
}
</style>
