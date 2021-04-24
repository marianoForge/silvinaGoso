<template>
  <section id="recent-projects" class="overflow-hidden">
    <v-row no-gutters>
      <v-col class=" text-center pa-5 white--text bg-section" cols="12" md="6">
        <base-bubble-1 style="transform: rotate(180deg) translateX(25%)" />

        <base-heading> Terapia de Pareja </base-heading>

        <base-text class="mb-12 px-10">
          Bajando nuestras barreras, hablar desde el corazón. <br /><br />
          Vamos y venimos entre nuestro ser vulnerables y reaccionar
          defensivamente cuando buscamos una y otra vez, conectar con la persona
          que queremos.<br /><br />
          Debajo de cada emoción reactiva y defensiva hay una emoción mucho más
          sensible que cuesta decodificar. Si descubrimos la vulnerabilidad como
          esa fuerza poderosa que nos conecta con los demás, y con nuestras
          necesidades y anhelos más profundos, vale el esfuerzo de darse tiempo
          y detenerse a explorarnos.
          <br /><br />Abrir el corazón hacia nosotros mismos o escuchar a los
          demás en esa sensibilidad, nos da la clave de cómo acercarnos y cómo
          generar una verdadera conexión amorosa.
        </base-text>

        <v-card color="secondary">
          <v-container class="pa-2">
            <v-row>
              <v-col
                v-for="project in projects"
                :key="project"
                cols="12"
                md="6"
              >
                <a href="#">
                  <v-img
                    :src="require(`@/assets/${project}.png`)"
                    max-height="300"
                  />
                </a>
              </v-col>
            </v-row>
          </v-container>
        </v-card>
      </v-col>

      <v-col class="hidden-sm-and-down" md="6">
        <v-img :src="require('@/assets/recentprojects.png')" height="100%" />
      </v-col>
    </v-row>
  </section>
</template>

<script>
export default {
  name: 'RecentProjects',

  data: () => ({
    projects: ['project1', 'project2', 'project3', 'project4'],
  }),
};
</script>

<style scoped>
.bg-section {
  background-color: blue;
}
</style>
