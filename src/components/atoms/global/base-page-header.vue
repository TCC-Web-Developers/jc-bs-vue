<template>
  <section class="page-header">
    <header class="bg-secondary">
      <div class="container d-flex align-items-center h-100">
        <div class="header-content text-center w-100">
          <slot name="page-header-name"></slot>
          <slot name="page-header-message"></slot>
        </div>
      </div>
    </header>
  </section>
</template>

<style lang="scss" scoped>
header {
  height: 45vh;
}
</style>
