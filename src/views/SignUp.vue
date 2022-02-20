<template>
  <div class="sign-up">
    <h1>Crie uma nova conta</h1>
    <input type="text" placeholder="Email" />
    <br />
    <br />
    <input type="password" placeholder="Senha" />
    <br />
    <br />
    <button>Registrar</button>
    <span>
      ou retorne ao
      <router-link to="/login">login.</router-link>
    </span>
  </div>
</template>

<script>
export default {
  name: "vue-registrar",
  data() {
    return {};
  },
  methods: {},
};
</script>

<style>
</style>