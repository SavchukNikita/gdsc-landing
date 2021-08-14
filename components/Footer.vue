<template lang="pug">
  v-footer( padless class="footer"  )
    v-card( tile flat  width="100%" class="footer__inner"  )
      v-card-text
        nav( role="navigation" )
          v-container(class="pa-0" )
            v-row( no-gutters justify="center"   class="footer__nav" )
              a(href="https://developers.google.com/community/gdg" class="text_body-1_medium footer__link" ) Google Developer Group
              a(href="https://gdgvl.ru/" class="text_body-1_medium footer__link") GDG Vladivostok
              a(href="https://developers.google.com/community/dsc" class="text_body-1_medium footer__link") Google Developer Students Club
              a(href="https://github.com/SavchukNikita/gdsc-landing" class="text_body-1_medium footer__link") Github
      v-card-text( class="text" ) {{ new Date().getFullYear() }} —
        |
        |
        strong GDSC Vladivostok
</template>

<style lang="scss" scoped>
  .footer {
    text-align: center;

    &__inner {
      background-color: var(--v-bg-secondary-base);
    }

    &__link {
      text-decoration: none;
      text-transform: uppercase;
      padding: 12px;
    }
  }
</style>
