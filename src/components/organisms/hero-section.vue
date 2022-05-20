<script setup>
import ImageContainer from "@/components/atoms/image-container.vue";
import HerosectionText from "@/components/atoms/herosection-text.vue";
import img from "@/assets/herosection-img.png";
</script>

<template>
  <div class="container">
    <div class="spacer"></div>
    <div class="herosection-container d-flex flex-column flex-md-row">
      <div class="right-section">
        <HerosectionText />
      </div>

      <div class="left-section">
        <ImageContainer :img="img" />
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@mixin display-center {
  display: flex;
  justify-content: center;
  align-items: center;
}

.spacer {
  height: 10vh;
}

.herosection-container {
  height: 90vh;

  .right-section {
    @include display-center;
    text-align: right;
    height: 100%;
    flex: 0.5;
  }

  .left-section {
    @include display-center;
    height: 100%;
    flex: 0.5;
  }
}
</style>
