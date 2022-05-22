<template>
  <section class="page-services">
    <div class="container">
      <ServiceItem :service="{ name: 'Design' }">
        <template v-slot:service-icon>
          <i
            class="bi bi-briefcase-fill text-secondary"
            style="font-size: 1.5rem"
          ></i>
        </template>
      </ServiceItem>
      <ServiceItem :service="{ name: 'Development' }">
        <template v-slot:service-icon>
          <i
            class="bi bi-code-slash text-secondary"
            style="font-size: 1.5rem"
          ></i>
        </template>
      </ServiceItem>
      <ServiceItem :service="{ name: 'Marketing' }">
        <template v-slot:service-icon>
          <i
            class="bi bi-gear-wide-connected text-secondary"
            style="font-size: 1.5rem"
          ></i>
        </template>
      </ServiceItem>
    </div>
  </section>
</template>
