<template>
  <v-app-bar
    v-scroll="onScroll"
    :color="!isScrolling ? 'transparent' : 'white'"
    fixed
    flat
  >
    <v-slide-x-transition>
      <v-img
        v-if="showLogo"
        :src="require('@/assets/logosilvina.png')"
        class="shrink"
        contain
        height="50"
        width="250"
      />
    </v-slide-x-transition>

    <v-spacer />

    <social-media />

    <base-btn
      class="ml-3"
      large
      href="https://store.vuetifyjs.com/product/freelancer-theme-free?ref=freelancer"
    >
      Agendá una Sesión

      <v-icon right small>
        mdi-open-in-new
      </v-icon>
    </base-btn>
  </v-app-bar>
</template>

<script>
import SocialMedia from "@/components/SocialMedia";
export default {
  name: "CoreAppBar",

  components: {
    SocialMedia,
  },

  data: () => ({
    showLogo: false,
    isScrolling: false,
  }),

  methods: {
    onScroll() {
      const offset = window.pageYOffset;
      this.isScrolling = offset > 50;
      this.showLogo = offset > 200;
    },
  },
};
</script>
