<template>
  <header class="section-header w-100 text-center">
    <h5 class="section-name text-accent"><slot name="section-name"></slot></h5>
    <slot name="section-message"></slot>
  </header>
</template>

<style lang="scss" scoped>
header {
  padding: 4rem 0;
}
</style>
