<template>
  <div>
    <v-btn
      v-for="(item, i) in items.slice(0, large ? items.length : 3)"
      :key="i"
      fab
      class="ma-2"
      color="info"
      :small="!large"
      v-bind:href="item.link"
    >
      <v-icon dark v-text="item.icon" />
    </v-btn>
  </div>
</template>

<script>
export default {
  props: {
    large: {
      type: Boolean,
      default: false,
    },
  },

  data: () => ({
    items: [
      {
        name: 'Instagram',
        icon: 'mdi-instagram',
        link: 'https://www.instagram.com/relaciones.emociones/',
      },

      {
        name: 'Email',
        icon: 'mdi-email',
        link: 'mailto:hola@relacionesyemociones.com',
      },
      {
        name: 'Phone',
        icon: 'mdi-phone',
        link: 'https://wa.link/3xp8lz',
      },
    ],
  }),
};
</script>
