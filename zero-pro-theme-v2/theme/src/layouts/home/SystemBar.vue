<template>
  <v-system-bar
    v-if="model"
    app
    color="#262626"
    class="px-4"
    dark
    height="58"
  >
    <a
      class="d-flex align-center"
      href="https://vuetifyjs.com/?ref=vtyd-pro-demo-system-bar"
      target="_blank"
    >
      <v-img
        alt="Vuetify Logo"
        class="mr-2"
        contain
        src="https://cdn.vuetifyjs.com/images/logos/vuetify-logo-dark.png"
        width="32"
      />

      <v-img
        alt="Vuetify Name"
        class="hidden-xs-only"
        contain
        width="96"
        src="https://cdn.vuetifyjs.com/images/logos/vuetify-name-dark.png"
      />
    </a>

    <v-spacer />

    <v-btn
      class="text-capitalize text-subtitle-2"
      color="success"
      href="https://store.vuetifyjs.com/products/zero-theme-pro/?ref=vtyd-system-bar"
      min-width="112"
    >
      Buy It Now
    </v-btn>

    <v-divider
      class="ml-6 mr-3"
      vertical
    />

    <v-btn
      class="text-capitalize grey--text mr-n2 mr-sm-n1"
      small
      text
      @click="model = false"
    >
      <v-icon
        color="white"
        :left="$vuetify.breakpoint.smAndUp"
      >
        mdi-close
      </v-icon>

      <span class="hidden-xs-only">
        Remove Frame
      </span>
    </v-btn>
  </v-system-bar>
</template>

<script>
  export default {
    name: 'HomeSystemBar',

    data: () => ({
      model: false,
    }),
  }
</script>
