<template>
  <v-row>
    <v-col class="text-center">
      <img src="/v.png" alt="Vuetify.js" class="mb-5" />
      <blockquote class="blockquote">
        &#8220;ABOUT&#8221;
        <footer>
          <small>
            <em>&mdash;John Johnson</em>
          </small>
        </footer>
      </blockquote>
    </v-col>
    <v-col>
      <v-text-field label="Outlined" outlined></v-text-field>
      <v-text-field placeholder="Search" outlined></v-text-field>
    </v-col>
  </v-row>
</template>

<script>
export default {
  data() {
    return {
      title: 'Tentang Kami',
    }
  },
}
</script>
