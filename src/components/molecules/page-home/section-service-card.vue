<template>
  <BaseCard class="base-card px-3 py-3" :color="'light'" :hover="true">
    <template v-slot:card-head>
      <BaseCardHead class="service-card-head py-4 px-2">
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
      <BaseCardFoot class="card-foot px-2 pb-4">
        <slot name="card-foot-content"></slot>
      </BaseCardFoot>
    </template>
  </BaseCard>
</template>

<style lang="scss" scoped></style>
