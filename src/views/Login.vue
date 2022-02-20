<template>
  <div class="vue-login">
    <h1>Login</h1>
    <input type="text" placeholder="Email" />
    <br />
    <br />
    <input type="password" placeholder="Senha" />
    <br />
    <div class="btn-login">
      <br />
      <button @click="login">Login</button>
    </div>
    <p>
      Você não tem conta?
      <span>
        <router-link to="/registrar">crie uma conta</router-link>
      </span>
    </p>
  </div>
</template>

<script>
export default {
  name: "vue-login",
  data() {
    return {};
  },
  methods: {
      login: function() {
          this.$router.replace("home");
      }
  }
};
</script>

<style scoped>
</style>