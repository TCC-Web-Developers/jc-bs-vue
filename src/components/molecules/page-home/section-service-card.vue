<template>
  <div class="service-card px-3 py-3">
    <BaseServiceCardHead>
      <BaseRoundedIcon :size="'3rem'" :color="'secondary'">
        <slot name="icon"></slot>
      </BaseRoundedIcon>
    </BaseServiceCardHead>
    <BaseServiceCardBody>
      <h4 class="service-card-title text-secondary fw-bold">
        <slot name="title"></slot>
      </h4>
      <p class="service-card-text"><slot name="text"></slot></p>
    </BaseServiceCardBody>
    <BaseServiceCardLink>
      <BaseLink :url="'#'" :style="'text-secondary'">Learn more</BaseLink>
    </BaseServiceCardLink>
  </div>
</template>

<style lang="scss" scoped>
.service-card {
  background-color: #fff;
  transition: 0.2s all linear;
  box-shadow: 0 4px 6px -1px rgb(0 0 0 / 0), 0 2px 4px -2px rgb(0 0 0 / 0);

  &:hover {
    transform: scale(1.04);
    box-shadow: 0 20px 25px -5px rgb(0 0 0 / 0.1),
      0 8px 10px -6px rgb(0 0 0 / 0.1);
  }
}
</style>
