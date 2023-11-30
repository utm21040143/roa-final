<template>
<v-row class="ma-0 pa-0 my-16" justify="center">
  <v-row class="pa-0 ma-0 mb-8" id="title-card" justify="center" align="center" style="width:100%">
    nos representan...
  </v-row>
  <v-row class="pa-0 ma-0" justify="center" style="width:100%">
    <v-col class="ma-0 pa-0" cols="4" v-for="(item, i) in card" :key="i">
      <v-card
        min-height="100%"
        class="ma-0 pa-0"
        color="dark"
        width="100%"
        tile
        elevation="0"
    >
        <v-card-text>
          <p class="text-h4 text--primary principal">
            {{item.title}}
          </p>

          <div class="text--primary principal">
          {{item.description}}<br>

          </div>
        </v-card-text>
        <v-img :width="300" cover :src="item.img" ></v-img>
      </v-card>
    </v-col>
  </v-row>
</v-row>
</template>

<script>
  export default {
    data: () => ({
      card:[
        {title: 'valores',
        description: 'Respeto por el medio ambiente: Nos comprometetemos a proteger el medio ambiente, utilizando prácticas agrícolas sostenibles.',
        },
        {title: 'un producto...',
        description: '...diferentes resultados',
        img:'durazno.png',
        },
        {title: 'el amor forma parte de nuestra historia',
        description: '',
        }
      ],

    }),
  }
</script>

