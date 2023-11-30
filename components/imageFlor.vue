<template>
  <v-row class="ma-0 pa-0" justify="center" style="width: 100%">
      <v-img
        :max-height="medida"
        max-width="auto"
        eager
        src="flor_peach.jpg"
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