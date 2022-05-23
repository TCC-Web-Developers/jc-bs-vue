<script setup>
import PortfolioImg from "@/assets/images/portfolio-img.jpg";
import ProductDesignImg from "@/assets/images/product-design-img.jpg";
import BlogImg from "@/assets/images/blog-img.jpg";

const projects = ref([
  {
    id: 0,
    title: "E-Commerce Design",
    text: `Lorem ipsum dolor, sit amet consectetur adipisicing elit. Similique, eaque!`,
    category: "UI/UX Design",
  },
  {
    id: 1,
    title: "Coffee Shop Branding",
    text: `Lorem ipsum dolor, sit amet consectetur adipisicing elit. Similique, eaque!`,
    category: "Product Design",
  },
  {
    id: 2,
    title: "Blogging Site",
    text: `Lorem ipsum dolor, sit amet consectetur adipisicing elit. Similique, eaque!`,
    category: "Web site",
  },
]);
</script>

<template>
  <section class="portfolio-section">
    <div class="container">
      <BaseSectionHeader>
        <template v-slot:section-name>PORTFOLIO </template>
        <template v-slot:section-message>
          <h1 class="display-5 section-message text-secondary">
            OUR LATEST WORK
          </h1>
        </template>
      </BaseSectionHeader>
      <div class="portfolio-container container">
        <div class="row">
          <div
            v-for="project in projects"
            :key="project.id"
            class="col-12 col-md-6 col-lg-4 portfolio-thumbnail mt-2"
          >
            <div class="wrapper">
              <div class="portfolio-card-inner-container">
                <SectionPortfolioCard>
                  <template v-slot:card-header-content>
                    <div class="thumbnail-img text-center">
                      <img ref="imgRef" :src="PortfolioImg" alt="img" />
                    </div>
                  </template>
                  <template v-slot:card-title>
                    <BaseCardTitle>
                      <BaseLink :url="'/#'" :style="'text-secondary'">{{
                        project.title
                      }}</BaseLink>
                    </BaseCardTitle>
                  </template>
                  <template v-slot:card-text>{{ project.text }} </template>
                  <template v-slot:card-foot-content>
                    <BaseCategoryLabel>{{
                      project.category
                    }}</BaseCategoryLabel>
                  </template>
                </SectionPortfolioCard>
              </div>
              <div class="thumbnail-body-background border shadow-sm"></div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.portfolio-section {
  .container {
    padding-bottom: 6rem;

    .portfolio-thumbnail {
      aspect-ratio: 1/1;
      position: relative;

      img {
        width: 100%;
        border-radius: 5px;
        transform: translateY(50%);
        transition: 0.3s all linear;
        box-shadow: 0 1px 3px 0 rgb(0 0 0 / 0.1),
          0 1px 2px -1px rgb(0 0 0 / 0.1);
      }

      &:hover {
        img {
          transform: translateY(0%);
          box-shadow: 0 20px 25px -5px rgb(0 0 0 / 0.1),
            0 8px 10px -6px rgb(0 0 0 / 0.1);
        }
      }

      .wrapper {
        position: relative;
        .portfolio-card-inner-container {
          position: relative;
          z-index: 6;
        }

        .thumbnail-body-background {
          position: absolute;
          bottom: 0;
          left: 0;
          width: 100%;
          height: 60%;
          background-color: #fff;
          border-radius: 5px;
          z-index: 5;
        }
      }

      // .thumbnail-body {
      //   position: relative;
      //   flex: 0.5;
      //   width: 100%;
      //   z-index: 5;

      //   .thumbnail-body-background {
      //     position: absolute;
      //     bottom: 0;
      //     left: 0;
      //     width: 100%;
      //     height: 150%;
      //     background-color: #fff;
      //     z-index: 6;
      //     border-radius: 5px;

      //     .thumbnail-content {
      //       position: absolute;
      //       bottom: 0;
      //       left: 50%;
      //       transform: translateX(-50%);
      //       width: 90%;
      //       height: 60%;

      //       .category {
      //         font-size: 0.8rem;
      //         width: max-content;
      //         border-radius: 100px;
      //       }
      //     }
      //   }
      // }
    }
  }
}
</style>
