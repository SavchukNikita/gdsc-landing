<template lang="pug">
  section( class="block about" id="about" )
    v-container
      v-row( no-gutters )
        v-col( cols="12" md="6" class="about__text"  )
          div( class="text_heading-3_regular _title" )
            span Developer  Students Club
            br
            span Vladivostok
          p( class="text mt-8 mb-0" ).
            Не просто ИТ-тусовка, а целая программа Google, созданная с целью погрузиться в мир информационных технологий, прокачать свои скилы и просто пообщаться в кругу  единомышленников.
          p( class="mt-8 mb-0" )
            a( class="v-btn btn__color_blue" href="https://developers.google.com/community/dsc" v-ripple  ) Больше о программе
        v-col( cols="12" md="6" class="about__img" align="center"  )
          img(src="../static/about-img.png", alt="fun pic" class="about__img-inner" )
</template>

<style lang="scss" scoped>
  .about {
    &__text {
      align-self: center;
    }
    &__img {
      align-self: center;

      &-inner {
        width: 80%;
        max-width: 460px;
        height: auto;
      }
    }
  }

  @media (max-width: 959px) {
    .about {
      &__text {
        margin-bottom: 32px;
      }

      &__img {
        &-inner {
          width: 100%;
        }
      }
    }
  }

  @media (max-width: 599px) {
    .about {
      &__img {
        order: -1;
      }
    }
  }
</style>
