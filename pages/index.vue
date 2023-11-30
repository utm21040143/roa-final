<template>
  <v-row class="ma-0 pa-0" justify="center" align="center" style="width:100%">
      <v-card width="100%" elevation="0" height="auto" color="transparent">
        <image-flor/>
        <card-uno/>
        <imagenes/>
        <valores-uno/>
      </v-card>
  </v-row>
</template>

<script>
import cardUno from '~/components/cardUno.vue';
export default {
  components: { cardUno },
};
</script>