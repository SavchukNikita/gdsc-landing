<template lang="pug">
  v-fab-transition
    v-btn( :key="icon" class="btn__color_blue" @click="switchTheme()"  fab icon fixed bottom right large )
          v-icon {{icon}}
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({

  computed: {
    icon () : String {
      if (this.$vuetify.theme.dark) {
        return 'mdi-weather-sunny'
      }

      return 'mdi-weather-night'
    }
  },
  methods: {
    switchTheme () {
      this.$vuetify.theme.dark = !this.$vuetify.theme.dark
      const theme = this.$vuetify.theme.dark ? 'dark' : 'light'
      window.localStorage.setItem('theme', theme)
    }
  }
})
</script>
