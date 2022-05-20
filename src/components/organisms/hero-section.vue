<script setup>
import ImageContainer from "@/components/atoms/image-container.vue";
import HerosectionText from "@/components/atoms/herosection-text.vue";
import img from "@/assets/herosection-img.png";
</script>

<template>
  <div class="herosection-container container">
    <div class="right-section">
      <HerosectionText />
    </div>

    <div class="left-section">
      <ImageContainer :img="img" />
    </div>
  </div>
</template>

<style lang="scss" scoped>
@mixin display-center {
  display: flex;
  justify-content: center;
  align-items: center;
}

.herosection-container {
  display: flex;
  height: 100vh;

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
