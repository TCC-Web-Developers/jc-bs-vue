<script setup>
import { ref } from "vue";
import ServiceContent from "@/components/organisms/service-page/service-content.vue";
import ProductDesignImage from "@/assets/images/product-design.jpg";
import CinematographyImage from "@/assets/images/cinematography.jpg";
import WebDesignImage from "@/assets/images/web-design.jpg";

const services = ref([
  {
    id: 0,
    title: "Product Design",
    text: `Lorem ipsum dolor sit, amet consectetur adipisicing elit. Assumenda
        possimus veniam animi, laboriosam sequi, consectetur est, similique
        molestiae vero rerum asperiores hic sit error eum voluptatibus ad? Ut
        quis hic reprehenderit rerum numquam saepe, eveniet tempore doloremque
        non excepturi cumque consequuntur, esse commodi odio cupiditate veniam
        consectetur deserunt mollitia nemo perspiciatis veritatis ratione magnam
        at? Sit sapiente accusamus magnam earum, molestias magni autem quas odio
        harum ea recusandae quasi consequatur iure debitis facilis adipisci,
        reprehenderit ex animi aliquam modi excepturi laborum, maxime
        consequuntur nostrum? Magnam quaerat vel quis sed mollitia totam dicta
        nihil aperiam earum perferendis odit in, minima rerum.`,
    imgUrl: ProductDesignImage,
  },
  {
    id: 1,
    title: "Cinematography",
    text: `        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Blanditiis
        aperiam, omnis fugit aliquam, nihil assumenda asperiores sed maxime non
        quasi dignissimos facilis? Exercitationem temporibus, quam at maiores
        voluptates ipsam, itaque obcaecati eum quidem dolorem nam magnam
        consectetur iusto tempore culpa expedita amet rerum vel quibusdam
        ratione! Iusto fugit dolore unde quibusdam, voluptas optio assumenda
        earum in nostrum doloremque laboriosam ipsum voluptate eligendi, quaerat
        aspernatur maiores maxime esse. Neque at eveniet eius quod earum
        voluptas quas suscipit quo aliquam, ab alias.`,
    imgUrl: CinematographyImage,
  },
  {
    id: 2,
    title: "Web Design",
    text: `        Lorem ipsum dolor sit amet consectetur adipisicing elit. Tempora ex
        distinctio velit architecto, temporibus perspiciatis omnis facilis
        quisquam numquam blanditiis, illum beatae atque sequi veniam maxime
        dolorum nisi ullam quam libero. Quae incidunt iste, corporis alias
        tenetur, dicta quaerat, non corrupti voluptate dolore deserunt aliquid
        voluptas maiores earum obcaecati eveniet.`,
    imgUrl: WebDesignImage,
  },
]);
</script>

<template>
  <main class="service-page w-100">
    <div class="container">
      <div class="title py-5">
        <h1 class="display-6 text-light">SERVICES</h1>
      </div>
      <div class="services">
        <ul>
          <li v-for="service in services" :key="service.id">
            <ServiceContent :serviceContent="service" />
          </li>
        </ul>
      </div>
    </div>
  </main>
</template>

<style lang="scss" scoped>
.card-img {
  display: block;
  width: 100%;
  height: 100%;
  object-fit: cover;
}
</style>
