<template>
  <v-row class="ma-0 pa-0" justify="center" style="width: 100%">
      <v-img
        lazy-src="https://media.istockphoto.com/id/1422874448/es/foto/agricultor-y-caja-llena-de-verduras-org%C3%A1nicas-cosecha-de-tomate-copiar-espacio.jpg?s=1024x1024&w=is&k=20&c=P_JiDINDb6gzLqkwLoluy4ZI9OnDfJIGk_5q10lAkY0="
        :max-height="medida"
        max-width="auto"
        eager
        src="https://media.istockphoto.com/id/1422874448/es/foto/agricultor-y-caja-llena-de-verduras-org%C3%A1nicas-cosecha-de-tomate-copiar-espacio.jpg?s=1024x1024&w=is&k=20&c=P_JiDINDb6gzLqkwLoluy4ZI9OnDfJIGk_5q10lAkY0="
      ></v-img>
  </v-row>
</template>

<script>
export default{
  data(){
    return{
      medida:0,
    }
  },
  mounted(){
    let size = Math.round(window.innerHeight);
    this.medida = size - 65
    this.medida = this.medida + 'px'
  }
}
</script>

