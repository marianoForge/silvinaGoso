<template>
  <section id="about" class="overflow-hidden">
    <v-row class="white" no-gutters>
      <v-col class="pa-5" cols="12" md="6">
        <base-bubble-1 style="transform: translate(5%, -5%)" />

        <base-heading class="info--text mb-7 ml-8">
          Mi Carrera
        </base-heading>

        <base-text class="mb-5 px-10">
          Tengo 30 años trabajando como psicóloga. Desde mis comienzos, mi
          interés estuvo en investigar y descubrir cómo los vínculos que vamos
          teniendo en la vida van modelando nuestra identidad. <br />
          Nacemos en relación y a partir del nacimiento, el amor desde y hacia
          los demás nos va delineando un camino en la vida en el que aprendemos
          y evolucionamos con otros significativos en nuestra historia.
        </base-text>
        <base-text class="mb-5 px-10">
          Hace 25 años, luego de haber iniciado mi práctica en orientación
          familiar de niños pequeños y parejas en etapa de gestación, comencé mi
          especialidad en Terapia Familiar Sistemica en CEFYP, y allí me formé y
          trabaje con familias y parejas por muchos años. Comprendo lo que
          significa en psicoterapia pensar el Ser en Relación y entender el
          sufrimiento humano a partir de los conflictos y la falta de claridad
          en su trama vincular. Integré allí distintos grupos de estudio con
          colegas, fui docente de postgrado, participé en congresos y
          presentaciones, e incluso en el libro de “Mas allá de pactos y
          traiciones”
        </base-text>
        <base-text class="mb-5 px-10">
          Desde mi base sistémica atendí muchas familias y parejas en el ámbito
          privado. También, comencé a trabajar en 1999 para Prosam/Osde, y
          realizo hasta la actualidad las entrevistas de orientación y
          derivación en el área de adultos, familias y parejas. He supervisado
          por años grupos de profesionales con distintas líneas teóricas, he
          dado conferencias, exposiciones en Jornadas institucionales y he
          coordinado paneles en presentaciones de profesionales.
        </base-text>
        <base-subheading class="info--text mt-8 ml-10">
          Mi Formación</base-subheading
        >

        <base-text class="mb-5 px-10">
          Mi formación, por mi curiosidad y pasión en mi profesion, se fue
          ampliando a medida que mi práctica fue creciendo. Me formé y entrené
          en <strong>EMDR</strong> para acceder y trabajar en experiencias
          traumáticas, profundicé en <strong>Hipnosis</strong> con el Dr.
          Scharovsky, explorando las profundidades del inconsciente. Realicé el
          entrenamiento y la práctica de Mindfulness e incursioné en prácticas
          chamánicas, y psicología transpersonal, lo que amplió mi mirada
          espiritual y conexión empática y sensible con mis pacientes. Pero en
          mis consultas, siguió siendo el eje ayudar a las personas a rediseñar
          y reconstruir su mundo emocional y vincular.
        </base-text>
        <base-text class="mb-5 px-10">
          Seguí mi formación en terapia de pareja con J.Gottman, luego con
          Leslie Greenberg, hasta que conocí a Sue Johnson y la
          <strong>TERAPIA FOCALIZADA EN LAS EMOCIONES</strong> ( de origen
          canadiense) donde hoy centro mi modelo de trabajo. Terminé mi
          formación en el 2015 con Sam Jinich, entrenador representante de habla
          hispana. Realicé el taller Hold me Tight en San Francisco, California
          y con mi socia Natalia Gilabert tradujimos y co-creamos Abrázame
          Fuerte Argentina, donde en talleres de fin de semana facilitamos la
          reconexión emocional en las parejas mediante una experiencia vivencial
          que crea sentido, fortaleciendo el amor. Hemos ofrecido este taller en
          Buenos Aires, Brasil y Chile. He colaborado en St. Louis, Missouri en
          el mismo formato organizado por la Lic. Peñalba para la comunidad
          Latina. Recientemente comenzamos a brindar la experiencia online.
        </base-text>

        <!-- <base-subheading class="info--text">
          Skills
        </base-subheading>

        <base-text class="mb-5">
          Lorem ipsum dolor sit amet, consecte tur adipi scin e<br />
          lit. Etiam vulputate augu e vel felis gravida porta.
        </base-text> -->

        <!-- <v-alert outlined color="info">
          <v-row v-for="(skill, i) in skills" :key="i" style="color: #69A1BB;">
            <v-col class="text-uppercase" cols="6" v-text="skill.name" />

            <v-col class="text-right" cols="6" v-text="`${skill.value}%`" />

            <v-progress-linear :value="skill.value" color="info" height="8" />
          </v-row>
        </v-alert> -->
      </v-col>

      <v-col class="hidden-sm-and-down" md="6">
        <v-img :src="require('@/assets/aboutme.png')" height="100%" />
      </v-col>
    </v-row>
  </section>
</template>

<script>
export default {
  data: () => ({
    skills: [
      {
        name: 'Web Design',
        value: 100,
      },
      {
        name: 'Web Development',
        value: 75,
      },
      {
        name: 'Web Support',
        value: 90,
      },
    ],
  }),
};
</script>
