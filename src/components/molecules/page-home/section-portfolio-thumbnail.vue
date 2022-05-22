<script setup>
import PortfolioImg from "@/assets/images/portfolio-img.jpg";
</script>

<template>
  <div class="col-12 col-md-6 col-lg-4 portfolio-thumbnail mt-2">
    <div class="thumbnail-img text-center">
      <slot name="thumbnail-img"></slot>
    </div>
    <div class="thumbnail-body">
      <div class="thumbnail-body-background border shadow-sm">
        <div
          class="thumbnail-content pb-3 d-flex flex-column justify-content-between"
        >
          <div class="thumbnail-title-text">
            <h5 class="thumbnail-title">
              <BaseLink :url="'/#'" :style="'text-secondary'"
                ><slot name="thumbnail-title"></slot
              ></BaseLink>
            </h5>
            <p><slot name="thumbnail-text"></slot></p>
          </div>
          <div class="thumbnail-category d-flex justify-content-center">
            <div
              class="category text-primary-text-light bg-secondary px-3 py-1"
            >
              <slot name="thumbnail-category"></slot>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
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
      box-shadow: 0 1px 3px 0 rgb(0 0 0 / 0.1), 0 1px 2px -1px rgb(0 0 0 / 0.1);
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
</style>
