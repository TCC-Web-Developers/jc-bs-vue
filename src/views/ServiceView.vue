<script setup></script>

<template>
  <main>
    <BasePageHeader>
      <template v-slot:page-header-name>
        <BasePageHeaderName>Services</BasePageHeaderName>
      </template>
      <template v-slot:page-header-message>
        <BasePageHeaderMessage>
          Agency provides a full service range including technical skills,
          design, business understanding.</BasePageHeaderMessage
        >
      </template>
    </BasePageHeader>
    <PageContent />
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
  </main>
</template>

<style lang="scss" scoped>
main {
  min-height: 200vh;
  width: 100%;

  header {
    height: 45vh;
  }
}
</style>
