<template>
  <header>
    <nav
      class="navbar navbar-expand-lg navbar-light bg-secondary position-fixed w-100"
    >
      <div class="container h-100 rounded-2">
        <BaseNavbarBrand>JC DESIGNS</BaseNavbarBrand>
        <NavLinks />
      </div>
    </nav>
  </header>
</template>

<style lang="scss" scoped>
nav {
  height: 10vh;
  box-shadow: 0 4px 6px -1px rgb(0 0 0 / 0.1), 0 2px 4px -2px rgb(0 0 0 / 0.1);
  z-index: 100;

  .container {
    height: 100%;
    padding: 0 1rem;
  }
}
</style>
