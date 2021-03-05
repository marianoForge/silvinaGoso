<template>
  <v-footer height="200" class="justify-center">
    <div class="text-center flex flex-col  ">
      <social-media large />
      <p class="font-bold mt-5">Silvina Goso - 2021</p>
    </div>
  </v-footer>
</template>

<script>
export default {
  name: 'CoreFooter',

  components: {
    SocialMedia: () => import('@/components/SocialMedia'),
  },
};
</script>
