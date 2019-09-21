<template>
  <v-app>
    <v-toolbar class="navbar py-5" color="transparent" flat absolute>
      <v-container class="d-flex">
        <img src="~assets/images/logo.png" alt="Noans" />
        <v-spacer />

        <v-toolbar-items class="d-none d-md-block">
          <v-btn v-scroll-reveal.reset="revealItem" text>Shop</v-btn>
          <v-btn v-scroll-reveal.reset="revealItem" text>Wholesale</v-btn>
          <v-btn v-scroll-reveal.reset="revealItem" text>Locations</v-btn>
          <v-btn v-scroll-reveal.reset="revealItem" text>Our Story</v-btn>
        </v-toolbar-items>
        <v-btn v-scroll-reveal.reset="revealItem" icon>
          <v-icon>mdi-magnify</v-icon>
        </v-btn>
        <v-btn v-scroll-reveal.reset="revealItem" icon>
          <v-icon>mdi-account-circle-outline</v-icon>
        </v-btn>
        <v-app-bar-nav-icon class="d-md-none"></v-app-bar-nav-icon>
      </v-container>
    </v-toolbar>

    <v-content> <nuxt /> </v-content>

    <v-footer dark>
      <v-container class="d-flex grey--text text--darken-1 font-weight-medium">
        <span>All rights Reserved &copy; 2019</span> <v-spacer />
        <span>+436 701 32 43 92</span>
      </v-container>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      revealItem: {
        distance: '50%',
        origin: 'right'
      }
    }
  }
}
</script>

<style lang="scss">
.navbar {
  width: 100%;
}
</style>
