<template>
  <v-app id="wim">
    <AppBar />

    <v-main>
      <Nuxt />
    </v-main>

    <AppFooter />
  </v-app>
</template>

<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator'

import AppBar from '~/components/AppBar.vue'
import AppFooter from '~/components/AppFooter.vue'

@Component({
  components: { AppBar, AppFooter },
})
export default class DefaultLayout extends Vue {}
</script>
