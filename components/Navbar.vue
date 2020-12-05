<template>
  <v-app-bar app color="white">
    <v-container class="py-0 fill-height" style="height: inherit">
      <v-btn class="page-link" text to="/" nuxt> Beranda </v-btn>
      <v-btn class="page-link" text to="/about" nuxt> Tentang Kami </v-btn>
      <v-btn class="page-link" text to="/product" nuxt> Produk </v-btn>
      <v-btn class="page-link" text to="/help-center" nuxt>
        Pusat Bantuan
      </v-btn>

      <v-spacer></v-spacer>
      <v-btn outlined color="primary">Masuk</v-btn>
      <v-btn depressed color="primary">Daftar</v-btn>
      <v-responsive max-width="260">
        <v-text-field
          prepend-inner-icon="fa-search"
          dense
          outlined
          hide-details
        ></v-text-field>
      </v-responsive>
    </v-container>
  </v-app-bar>
</template>

<style lang="scss">
.v-app-bar {
  &.v-btn--active {
    font-weight: 600;
    color: red;
  }
  .page-link {
    height: 100% !important;
    border-radius: 0 !important;
  }
}

.v-toolbar__content,
.v-toolbar__extension {
  padding-top: 0;
  padding-bottom: 0;
}
</style>
