<script setup>
import BaseServiceContent from "@/components/base-service-content.vue";
import ProductDesignImage from "@/assets/images/product-design.jpg";
import BaseContentImage from "@/components/atoms/service-page/base-content-image.vue";
import BaseContentText from "@/components/atoms/service-page/base-content-text.vue";
import BaseContentTitle from "@/components/atoms/service-page/base-content-title.vue";
</script>

<template>
  <BaseServiceContent>
    <template v-slot:service-content-image>
      <BaseContentImage :img="ProductDesignImage" />
    </template>
    <template v-slot:service-content-title>
      <BaseContentTitle>Product Designs</BaseContentTitle>
    </template>
    <template v-slot:service-content-text>
      <BaseContentText>
        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Assumenda
        possimus veniam animi, laboriosam sequi, consectetur est, similique
        molestiae vero rerum asperiores hic sit error eum voluptatibus ad? Ut
        quis hic reprehenderit rerum numquam saepe, eveniet tempore doloremque
        non excepturi cumque consequuntur, esse commodi odio cupiditate veniam
        consectetur deserunt mollitia nemo perspiciatis veritatis ratione magnam
        at? Sit sapiente accusamus magnam earum, molestias magni autem quas odio
        harum ea recusandae quasi consequatur iure debitis facilis adipisci,
        reprehenderit ex animi aliquam modi excepturi laborum, maxime
        consequuntur nostrum? Magnam quaerat vel quis sed mollitia totam dicta
        nihil aperiam earum perferendis odit in, minima rerum.
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
