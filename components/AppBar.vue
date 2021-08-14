<template lang="pug">
  v-app-bar.appbar( app :elevate-on-scroll="!$vuetify.theme.isDark" )
    v-container
      v-row( no-gutters align="center" )
        img.appbar__logo.pr-3(src="../assets/images/gdsc-logo.png" alt="GDSC logo" v-show="!$vuetify.breakpoint.xs" )
        v-toolbar-title
          span {{$vuetify.breakpoint.xs ? 'GDSC Vladivostok' : 'Google Developer Students Club'}}
        v-spacer
        nav( role='navigation' v-if="!$vuetify.breakpoint.mobile" )
          a(href="#about" class="appbar__link text_body-1_medium" ) О нас
          a(href="#events" class="appbar__link text_body-1_medium" ) Мероприятия
          a(href="#broadcasts" class="appbar__link text_body-1_medium" ) Трансляции
          a(href="#feedback" class="appbar__link text_body-1_medium" ) Обратная связь
        v-app-bar-nav-icon( v-else )
</template>

<style lang="scss" scoped>
  .appbar {
    background-color: var(--v-primary-base) !important;

    &__logo {
      max-width: 50px;
      height: auto;
    }

    &__link {
      padding: 12px;
      text-decoration: none;
    }

    & .v-toolbar__content {
      padding-left: 0;
      padding-right: 0;
    }
  }
</style>
