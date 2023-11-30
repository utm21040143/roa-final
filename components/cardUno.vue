<template>
  <v-card class="card1">
    <v-list-item three-line v-for="(item, i) in text" :key="i">
      <v-list-item-content>
        <div class="text-overline mb-4">
          EN ROA
        </div>
        <v-list-item-title class="text-h5 mb-6">
          somos
        </v-list-item-title>
        <v-row class="ma-0 pa-0 text-card">
        {{item.description}}
        </v-row>
      </v-list-item-content>
    </v-list-item>
  </v-card>
</template>

<script>
  export default {
    data: () => ({
      text:[
        {
        description: 'Una familia ##### llevamos más de 50 años cultivando duraznos en el corazón de Aguascalientes, México. Nuestra pasión por la fruta y nuestro compromiso con la calidad nos han convertido en uno de los principales productores de duraznos del país. Nuestros duraznos se cultivan en huertos cuidadosamente seleccionados, utilizando prácticas agrícolas sostenibles. Recogemos los duraznos a mano en su punto óptimo de maduración, para garantizar que nuestros clientes disfruten de una fruta deliciosa y fresca. Ofrecemos una variedad de duraznos, incluyendo duraznos amarillos, duraznos blancos y duraznos de cereza. Todos nuestros duraznos son 100% naturales y sin conservantes',
        },
      ],

    }),
  }
</script>