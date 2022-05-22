<script setup>
const navLinks = ref([
  {
    id: 0,
    name: "Home",
    url: "/",
  },
  {
    id: 1,
    name: "Service",
    url: "/service",
  },
  {
    id: 2,
    name: "About",
    url: "/about",
  },
]);
</script>

<template>
  <ul class="navlinks d-flex align-items-center h-100">
    <BaseNavbarLink
      v-for="navLink in navLinks"
      :key="navLink.id"
      :url="navLink.url"
      >{{ navLink.name }}</BaseNavbarLink
    >
  </ul>
</template>

<style lang="scss" scoped>
ul {
  list-style: none;
  margin: 0;
  padding: 0;
}
</style>
