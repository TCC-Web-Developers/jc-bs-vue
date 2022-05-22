<script setup></script>

<template>
  <div class="root-app">
    <NavigationBar />
    <div class="spacer bg-secondary"></div>
    <RouterView />
    <FooterSection />
  </div>
</template>

<style lang="scss">
@import "./assets/scss/custom.scss";
.spacer {
  height: 10vh;
  width: 100%;
}
</style>
