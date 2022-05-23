<template>
  <BaseCard
    class="base-card px-3 pb-2"
    :color="'transparent'"
    :fixedSize="true"
  >
    <template v-slot:card-head>
      <BaseCardHead class="service-card-head">
        <slot name="card-header-content"></slot>
      </BaseCardHead>
    </template>
    <template v-slot:card-body>
      <BaseCardBody class="card-body px-2">
        <slot name="card-title"></slot>
        <slot name="card-text"></slot>
      </BaseCardBody>
    </template>
    <template v-slot:card-foot>
      <BaseCardFoot
        class="card-foot px-2 pb-2 pt-4 d-flex justify-content-center"
      >
        <slot name="card-foot-content"></slot>
      </BaseCardFoot>
    </template>
  </BaseCard>
</template>

<style lang="scss" scoped>
// .portfolio-thumbnail {
//   aspect-ratio: 1/1;
//   display: flex;
//   flex-direction: column;

//   .thumbnail-img {
//     position: relative;
//     z-index: 7;
//     flex: 0.5;

//     img {
//       width: 90%;
//       border-radius: 5px;
//       transform: translateY(50%);
//       transition: 0.3s all linear;
//       box-shadow: 0 1px 3px 0 rgb(0 0 0 / 0.1), 0 1px 2px -1px rgb(0 0 0 / 0.1);
//     }
//   }

//   &:hover {
//     img {
//       transform: translateY(0%);
//       box-shadow: 0 20px 25px -5px rgb(0 0 0 / 0.1),
//         0 8px 10px -6px rgb(0 0 0 / 0.1);
//     }
//   }

//   .thumbnail-body {
//     position: relative;
//     flex: 0.5;
//     width: 100%;
//     z-index: 5;

//     .thumbnail-body-background {
//       position: absolute;
//       bottom: 0;
//       left: 0;
//       width: 100%;
//       height: 150%;
//       background-color: #fff;
//       z-index: 6;
//       border-radius: 5px;

//       .thumbnail-content {
//         position: absolute;
//         bottom: 0;
//         left: 50%;
//         transform: translateX(-50%);
//         width: 90%;
//         height: 60%;

//         .category {
//           font-size: 0.8rem;
//           width: max-content;
//           border-radius: 100px;
//         }
//       }
//     }
//   }
// }
</style>
