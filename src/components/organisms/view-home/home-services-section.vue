<script setup>
const services = ref([
  {
    id: 0,
    title: "Design",
    text: `Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eum quia, id repellendus vitae maiores atque.`,
    icon: "bi-briefcase-fill",
  },
  {
    id: 1,
    title: "Development",
    text: `Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eum quia, id repellendus vitae maiores atque.`,
    icon: "bi-code-slash",
  },
  {
    id: 2,
    title: "Marketing",
    text: `Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eum quia, id repellendus vitae maiores atque.`,
    icon: "bi-gear-wide-connected",
  },
]);
</script>

<template>
  <section class="services-section bg-primary">
    <div class="background-color-design bg-secondary"></div>
    <div class="container service-foreground">
      <BaseSectionHeader>
        <template v-slot:section-name>SERVICES </template>
        <template v-slot:section-message>
          <h1 class="display-5 section-message text-primary">
            HOW CAN I HELP YOU?
          </h1>
        </template>
      </BaseSectionHeader>
      <div class="services-container">
        <div class="row">
          <div
            v-for="service in services"
            :key="service.id"
            class="col-12 border-bottom border-md-0 col-md-4 px-0"
          >
            <SectionServiceCard>
              <template v-slot:card-header-content>
                <BaseRoundedIcon :size="'3rem'" :color="'secondary'">
                  <i
                    :class="`bi ${service.icon} text-primary`"
                    style="font-size: 1.5rem"
                  ></i>
                </BaseRoundedIcon>
              </template>
              <template v-slot:card-title>
                <BaseCardTitle>{{ service.title }}</BaseCardTitle>
              </template>
              <template v-slot:card-text>
                <BaseCardText>{{ service.text }} </BaseCardText>
              </template>
              <template v-slot:card-foot-content>
                <BaseLink :url="'#'" :style="'text-secondary'"
                  >Learn more</BaseLink
                >
              </template>
            </SectionServiceCard>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.services-section {
  background-color: #fff;
  position: relative;

  .service-foreground {
    position: relative;
    z-index: 5;
    padding: 6rem 0;

    .services-container {
      background-color: green;
    }
  }

  .background-color-design {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 70%;
    z-index: 0;
  }
}
</style>
