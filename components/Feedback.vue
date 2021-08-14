<template lang="pug">
  section( class="block feedback" id="feedback" )
    v-container
      v-row( no-gutters )
        v-col( align="center" class="feedback__title title_spacer" cols="12" md="6" )
          h2(class="_title text_heading-3_regular") Для нетсталкеров
        v-col( cols="12" md="6" )
          v-row( no-gutters align="center" justify="center" )
            .feedback__img
              a(href="https://t.me/vldscfefu")
                img(src="../static/telegram.png" alt="telegram" class="feedback__img-inner" )
            .feedback__img
              a(href="https://vk.com/vldsc")
                img(src="../static/vk.png" alt="vk" class="feedback__img-inner" )
</template>

<style lang="scss" scoped>
  .feedback {
    &__img {
      margin: 12px 24px;
      max-width: 150px;
      width: 30%;

      &-inner {
        max-width: 150px;
        width: 100%;
        height: auto;
      }
    }

    &__title {
      align-self: center;
    }
  }

  @media (min-width: 960px) {
    .feedback {
      &__title {
        margin-bottom: 0;
      }
    }
  }
</style>
