<template>
  <div class="login">
    <form @submit.prevent="login">
      <label for="email">Email:</label>
      <input id="email" v-model="email" type="email" required>

      <label for="password">Password:</label>
      <input id="password" v-model="password" type="password" required>
      <button type="submit">
        Login
      </button>
    </form>
  </div>
</template>

<script>
export default {
  data () {
    return {
      email: '',
      password: ''
    }
  },
  methods: {
    login () {
      console.log('Login:', this.email, this.password)
    }
  }
}
</script>
