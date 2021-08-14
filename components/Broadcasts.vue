<template lang="pug">
  section( class="block block_spacer broadcasts" id="broadcasts")
    v-container
      .title_spacer
        h2(class="_title broadcasts__title text_heading-3_regular" ) Трансляции
        h3( class="broadcasts__subtitle text_subtitle-1_regular mt-2" ) Чтобы ничего не упустить и оставаться в теме

      v-row( no-gutters class="broadcasts__items" justify="center" )
        BroadcastItem
        BroadcastItem
        BroadcastItem
        BroadcastItem
        BroadcastItem
</template>

<style lang="scss" scoped>
  .broadcasts {
    &__title, &__subtitle {
      text-align: center;
    }
  }
</style>
