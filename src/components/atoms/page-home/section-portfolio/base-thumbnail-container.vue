<template>
  <div class="thumbnail-img text-center">
    <slot></slot>
  </div>
</template>

<style lang="scss" scoped>
.thumbnail-img {
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  z-index: 7;
  flex: 0.5;
}
</style>
