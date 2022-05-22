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
          <div class="col-12 border-bottom border-md-0 col-md-4 px-0">
            <SectionServiceCard>
              <template v-slot:icon>
                <i
                  class="bi bi-briefcase-fill text-primary"
                  style="font-size: 1.5rem"
                ></i>
              </template>
              <template v-slot:title>Design</template>
              <template v-slot:text>
                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eum
                quia, id repellendus vitae maiores atque.
              </template>
            </SectionServiceCard>
          </div>
          <div class="col-12 border-bottom border-md-0 col-md-4 px-0">
            <SectionServiceCard>
              <template v-slot:icon>
                <i
                  class="bi bi-code-slash text-primary"
                  style="font-size: 1.5rem"
                ></i>
              </template>
              <template v-slot:title>Design</template>
              <template v-slot:text>
                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eum
                quia, id repellendus vitae maiores atque.
              </template>
            </SectionServiceCard>
          </div>
          <div class="col-12 border-bottom border-md-0 col-md-4 px-0">
            <SectionServiceCard>
              <template v-slot:icon>
                <i
                  class="bi bi-gear-wide-connected text-primary"
                  style="font-size: 1.5rem"
                ></i>
              </template>
              <template v-slot:title>Design</template>
              <template v-slot:text>
                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eum
                quia, id repellendus vitae maiores atque.
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
