<template>
  <section id="services" class="overflow-hidden">
    <v-row class="accent" no-gutters>
      <v-col class="hidden-sm-and-down" md="6">
        <v-img :src="require('@/assets/services.png')" height="100%" />
      </v-col>

      <v-col class="text-center pa-5" cols="12" md="6">
        <v-row class="fill-height" align="center" justify="center">
          <v-col cols="12">
            <base-bubble-2 style="transform: translateX(55%)" />
            <base-heading class="info--text">
              ¿Cómo te puedo ayudar?
            </base-heading>

            <!-- <base-text class="mb-5">
              Curabitur venenatis tortor erat, quis laoreet nis<br />
              lobortis eget. Fusce tempor aucto.
            </base-text> -->
          </v-col>

          <v-col
            v-for="(service, i) in services"
            :key="i"
            class="text-center mb-3"
            md="6"
          >
            <v-avatar class="elevation-6 mb-2" color="#69A1BB" size="64" tile>
              <v-icon dark size="52" v-text="service.icon" />
            </v-avatar>

            <base-text>
              <div class="mb-2 font-bold" v-html="service.name" />
              <div v-html="service.blurb" />
            </base-text>
          </v-col>
        </v-row>
      </v-col>
    </v-row>
  </section>
</template>

<script>
export default {
  name: 'Services',

  data: () => ({
    services: [
      {
        name: '<b>Supervisión Profesional</b>',
        icon: 'mdi-clipboard-text-outline',
        blurb:
          'Si sos terapeuta, puedo acompañarte en tu desarrollo profesional ',
      },
      {
        name: '<b>Rediseñando tus vínculos</b>',
        icon: 'mdi-pencil-outline',
        blurb: 'Sesiones para construir </br>vínculos más seguros',
      },
      {
        name: '<b>Talleres TFE </b>',
        icon: 'mdi-settings-outline',
        blurb:
          '<b>Para parejas</b>: Abrázame Fuerte Argentina. <b>Entrenamientos Para profesionales</b>: Externship y CoreSkills 1-2',
      },
      {
        name: '<b>Terapia de Pareja</b>',
        icon: 'mdi-account',
        blurb:
          'Abriendo paso a la vulnerabilidad </br>como herramienta para</br> la conexión amorosa',
      },
    ],
  }),
};
</script>
