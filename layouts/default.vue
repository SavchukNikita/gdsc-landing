<template lang="pug">
  v-app
    AppBar
    v-main
      v-container( fluid )
        Nuxt
    Footer
    ThemeSwitcher
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  mounted () {
    const theme = window.localStorage.getItem('theme')
    const isDark = theme !== 'light'

    // ! Баг фреймворка. Без обертки setTimeout не работают некоторые стили
    // eslint-disable-next-line no-return-assign
    setTimeout(() => this.$vuetify.theme.dark = isDark, 0)
  }
})
</script>
