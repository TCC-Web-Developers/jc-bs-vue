<script setup>
import PortfolioImg from "@/assets/images/portfolio-img.jpg";
import ProductDesignImg from "@/assets/images/product-design-img.jpg";
import BlogImg from "@/assets/images/blog-img.jpg";
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
          <SectionPortfolioThumbnail>
            <template v-slot:thumbnail-img>
              <img ref="imgRef" :src="PortfolioImg" alt="img" />
            </template>
            <template v-slot:thumbnail-title> E-commerce Website </template>
            <template v-slot:thumbnail-text>
              Lorem ipsum dolor, sit amet consectetur adipisicing elit.
              Similique, eaque!
            </template>
            <template v-slot:thumbnail-category>UI/UX Design </template>
          </SectionPortfolioThumbnail>
          <SectionPortfolioThumbnail>
            <template v-slot:thumbnail-img>
              <img ref="imgRef" :src="ProductDesignImg" alt="img" />
            </template>
            <template v-slot:thumbnail-title> Coffee Shop Branding </template>
            <template v-slot:thumbnail-text>
              Lorem ipsum dolor, sit amet consectetur adipisicing elit.
              Similique, eaque!
            </template>
            <template v-slot:thumbnail-category>Product Design </template>
          </SectionPortfolioThumbnail>
          <SectionPortfolioThumbnail>
            <template v-slot:thumbnail-img>
              <img ref="imgRef" :src="BlogImg" alt="img" />
            </template>
            <template v-slot:thumbnail-title> Blogging Site </template>
            <template v-slot:thumbnail-text>
              Lorem ipsum dolor, sit amet consectetur adipisicing elit.
              Similique, eaque!
            </template>
            <template v-slot:thumbnail-category>Web development </template>
          </SectionPortfolioThumbnail>
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
      display: flex;
      flex-direction: column;

      .thumbnail-img {
        position: relative;
        z-index: 7;
        flex: 0.5;

        img {
          width: 90%;
          border-radius: 5px;
          transform: translateY(50%);
          transition: 0.3s all linear;
          box-shadow: 0 1px 3px 0 rgb(0 0 0 / 0.1),
            0 1px 2px -1px rgb(0 0 0 / 0.1);
        }
      }

      &:hover {
        img {
          transform: translateY(0%);
          box-shadow: 0 20px 25px -5px rgb(0 0 0 / 0.1),
            0 8px 10px -6px rgb(0 0 0 / 0.1);
        }
      }

      .thumbnail-body {
        position: relative;
        flex: 0.5;
        width: 100%;
        z-index: 5;

        .thumbnail-body-background {
          position: absolute;
          bottom: 0;
          left: 0;
          width: 100%;
          height: 150%;
          background-color: #fff;
          z-index: 6;
          border-radius: 5px;

          .thumbnail-content {
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 90%;
            height: 60%;

            .category {
              font-size: 0.8rem;
              width: max-content;
              border-radius: 100px;
            }
          }
        }
      }
    }
  }
}
</style>
