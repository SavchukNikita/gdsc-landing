<template lang="pug">
  section( class="block_darken block_spacer events" id="events" )
    v-container
      .title_spacer
        h2( class="events__title _title text_heading-3_regular" ) Мероприятия
        h3( class="events__subtitle text_subtitle-1_regular mt-2" ) Подгоняй знакомиться, общаться и учиться
      SingleEvent
</template>

<style lang="scss" scoped>
  .events {
    &__title, &__subtitle {
      text-align: center;
    }
  }
</style>
