<template>
  <section id="welcome" class="overflow-hidden">
    <v-row no-gutters>
      <v-col class="hidden-sm-and-down" md="6">
        <v-img :src="require('@/assets/welcome.png')" />
      </v-col>

      <v-col
        class="align-content-space-between layout wrap"
        cols="12"
        md="6"
        :pa-5="$vuetify.breakpoint.smAndDown"
      >
        <base-bubble-1 style="transform: rotate(180deg) translateY(25%)" />

        <v-row align="center" justify="center">
          <v-col cols="10" md="6">
            <base-heading>Hola! Soy Silvina Goso</base-heading>
            <base-text>
              Psicóloga clínica y terapeuta de parejas con formación en Terapia
              Focalizada en las Emociones (TFE).<br /><br />
              Durante mis más de 25 años como terapeuta he ayudado a más de 500
              parejas a rediseñar sus vínculos para vivir una relación de pareja
              sana y segura. También he participado en la formación de más de
              150 psicólogos en los últimos 5 años durante los talleres del
              Externship y Core Skills de TFE en Argentina, Brasil y Estados
              Unidos para poder ayudar a que más personas puedan construir sus
              vínculos seguros.
            </base-text>
            <base-btn class="mt-4">
              ¡Conversemos!
            </base-btn>
          </v-col>
        </v-row>

        <base-bubble-2
          style="transform: rotate(180deg) translate(-200px, -15%)"
        />
      </v-col>
    </v-row>
  </section>
</template>
