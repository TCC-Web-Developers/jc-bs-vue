<template>
  <BaseCard
    class="base-card px-3 py-3"
    :color="'light'"
    :shadow="'shadow-sm'"
    :fixedSize="true"
  >
    <template v-slot:card-head>
      <BaseCardHead class="service-card-head">
        <slot name="card-header-content"></slot>
      </BaseCardHead>
    </template>
    <template v-slot:card-body>
      <BaseCardBody class="card-body px-2">
        <slot name="card-title"></slot>
        <slot name="card-text"></slot>
      </BaseCardBody>
    </template>
    <template v-slot:card-foot>
      <BaseCardFoot
        class="card-foot px-2 pb-2 pt-4 d-flex justify-content-center"
      >
        <slot name="card-foot-content"></slot>
      </BaseCardFoot>
    </template>
  </BaseCard>
</template>

<style lang="scss" scoped></style>
