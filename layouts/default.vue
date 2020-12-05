<template>
  <v-app id="app">
    <Navbar />
    <v-main class="">
      <v-container>
        <nuxt />
      </v-container>
    </v-main>
    <Footer />
  </v-app>
</template>

<script>
import Navbar from '~/components/Navbar.vue'
import Footer from '~/components/Footer.vue'

export default {
  name: 'App',
  components: {
    Navbar,
    Footer,
  },
  head() {
    const url = 'https://travelaja.id' + this.$route.path
    return {
      link: [
        {
          rel: 'travelaja',
          href: url,
        },
      ],
      meta: [{ property: 'og:url', content: url }],
    }
  },
}
</script>
