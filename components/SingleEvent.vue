<template lang="pug">
  .single-event
    v-row( no-gutters )
      v-col( cols="12" md="6" align="center" class="single-event__img"   )
          img(src="../static/single-event.png", alt="event" class="single-event__img-inner" )
      v-col( cols="12" md="6" )
        div( class="single-event__title _title text_heading-4_regular" )
          span DevFest 2077
        p( class="text mt-8 mb-0" ).
          Отличный нетворкинг с интересными людьми, которые говорят с тобой на одном языке.
          Эксклюзивная информация от мощнейших IT-специалистов со всей России и не только.
          Последние разработки и новейшие технологии Google
        p( class="text_body-1_medium mt-8 mb-0" ) 2 октября 2021, 10:00, Арена Экспо
        v-col( sm="3" md="12" class="pa-0 mt-8" )
          a( class="single-event__btn-more v-btn btn__color_blue" v-ripple) Подробнее
</template>

<style lang="scss" scoped>
  .single-event {
    &__img {
      align-self: center;

      &-inner {
        width: 40%;
        max-width: 200px;
        height: auto;
      }
    }

    &__title {
      text-align: center;
    }

    &__btn-more {
      width: 100%;
    }
  }

  @media (max-width: 959px) {
    .single-event {
      &__img {
        margin-bottom: 32px;
      }
    }
  }
</style>
