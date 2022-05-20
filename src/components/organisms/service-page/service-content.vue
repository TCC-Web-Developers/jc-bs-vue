<script setup>
import BaseServiceContent from "@/components/base-service-content.vue";

// import BaseContentImage from "@/components/atoms/service-page/base-content-image.vue";
// import BaseContentText from "@/components/atoms/service-page/base-content-text.vue";
// import BaseContentTitle from "@/components/atoms/service-page/base-content-title.vue";
import BaseContentImage from "@/components/service-page-atoms/base-content-image.vue";
import BaseContentText from "@/components/service-page-atoms/base-content-text.vue";
import BaseContentTitle from "@/components/service-page-atoms/base-content-title.vue";

const props = defineProps(["serviceContent"]);
</script>

<template>
  <BaseServiceContent>
    <template v-slot:service-content-image>
      <BaseContentImage :img="serviceContent.imgUrl" />
    </template>
    <template v-slot:service-content-title>
      <BaseContentTitle>{{ serviceContent.title }}</BaseContentTitle>
    </template>
    <template v-slot:service-content-text>
      <BaseContentText>
        {{ serviceContent.text }}
      </BaseContentText>
    </template>
  </BaseServiceContent>
</template>

<style lang="scss" scoped>
.card-img {
  display: block;
  width: 100%;
  height: 100%;
  object-fit: cover;
}
</style>
