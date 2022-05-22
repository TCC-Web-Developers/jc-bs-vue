<template>
  <section class="page-content py-5">
    <div class="container d-flex py-5">
      <div class="content-title w-50">
        <slot name="page-content-name"></slot>
        <slot name="page-content-heading"></slot>
      </div>
      <div class="content-text w-50">
        <slot name="page-content-text"></slot>
      </div>
    </div>
  </section>
</template>
