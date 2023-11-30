<template>
  <v-app ligth>
    <v-main>
    <headerApp/>
    <Nuxt style="margin-top:56px !important; width:100%"/>
    <v-footer style="width:100%; justify-content: center;">
      <footer-app/>
    </v-footer>
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: 'DefaultLayout',
  data () {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Inicio',
          to: '/'
        },
        {
          icon: 'mdi-account',
          title: 'Inicio de Sesión',
          to: '/login'
        },
        {
          icon: 'mdi-calendar',
          title: 'Calendario',
          to: '/system_in'
        }
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'ROA'
    }
  }
}
</script>
