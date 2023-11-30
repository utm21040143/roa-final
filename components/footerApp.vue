<template>
  <v-footer color="dark" padless max-width="100%">
    <v-row justify="center" no-gutters>
      <router-link to="/">
        <v-btn color="white" text rounded class="my-2"> Inicio </v-btn>
      </router-link>
      <v-btn
        v-for="link in links"
        :key="link"
        color="white"
        text
        rounded
        class="my-2"
      >
        {{ link }}
      </v-btn>
      <router-link to="/login">
        <v-btn color="white" text rounded class="my-2"> Admin </v-btn>
      </router-link>
      <v-col class="lighten-2 py-4 text-center white--text" cols="12">
        {{ new Date().getFullYear() }} —
        <strong>Tlamaki Professional Services</strong>
      </v-col>
    </v-row>
  </v-footer>
</template>

<script>
export default {
  data: () => ({
    links: ['Sobre Nosotros', 'Contacto'],
  }),
}
</script>
