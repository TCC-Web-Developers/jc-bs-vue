<script setup></script>

<template>
  <div class="card mb-5 w-100">
    <div class="row g-0">
      <div class="col-md-4">
        <slot name="service-content-image"></slot>
      </div>
      <div class="col-md-8">
        <div class="card-body">
          <slot name="service-content-title"></slot>
          <slot name="service-content-text"></slot>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped></style>
