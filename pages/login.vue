<template>
  <v-row class="ma-0 pa-0 pa-3" justify="center" style="width:100%;height:calc(100dvh - 176px) !important;" id="sapo">
    <v-img src="fondoLogin1.jpg" style="min-width: 100%; max-height:calc(100dvh - 176px) !important; min-height:calc(100dvh - 176px) !important; position: absolute;"></v-img>
    <v-card class="ma-0 pa-0 pa-6" width="400px" color="transparent" elevation="0" height="100%">
       <v-row class="ma-0 pa-0" justify="center" style="height:100%; display: flex; align-content: center;">
          <v-row class="ma-0 mb-3" style="width:100%" justify="center">
            Bienvenido
          </v-row>
          <hr style="width:100%;">
          <v-row class="ma-0" style="width:100%; margin: 12px 0 !important" justify="center">
            <v-col class="pa-0" cols="6">
              <v-row class="ma-0" style="width:100%" justify="center">
                olvidaste
              </v-row>
            </v-col>
            <v-col class="pa-0" cols="6">
              <v-row class="ma-0" style="width:100%" justify="center">
                registrate
              </v-row>
            </v-col>
          </v-row>
          <hr style="width:100%;">
          <v-row class="ma-0 mt-4" style="width:100%" justify="center">
            <v-text-field hide-details="true" label="Outlined" placeholder="Placeholder" outlined dense >
            </v-text-field>
          </v-row>
          <v-row class="ma-0 mt-4" style="width:100%" justify="center">
            <v-text-field v-model="password" outlined dense hide-details :append-icon="show ? 'mdi-eye' : 'mdi-eye-off'" :rules="[rules.required, rules.min]" :type="show ? 'text' : 'password'" label="Contraseña" @click:append="show = !show">
            </v-text-field>
          </v-row>
       </v-row>
    </v-card>
  </v-row>
</template>

<script>
export default {
  data() {
    return {
      usuario: '',
      password: '',
      password: 'Password',
      show: false,
      rules: {
        required: value => !!value || 'Required.',
        min: v => v.length >= 8 || 'Min 8 characters',
        emailMatch: () => (`The email and password you entered don't match`),
      },
    }
  },

  methods: {
    onSubmit() {
      if (!this.usuario || !this.password) {
        alert('Ingrese ambos campos para iniciar sesión.')
        return
      }

      console.log('Form submitted: ', {
        usuario: this.usuario,
        password: this.password,
      })
    },
  },
}
</script>


