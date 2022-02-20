<template>
  <div class="vue-login">
    <Root>
      <H1>Login</H1>
      <Input type="text" placeholder="Email" />
      <br />
      <br />
      <Input type="password" placeholder="Senha" />
      <br />
      <div class="btn-login">
        <br />
        <Button @click="login">Login</Button>
      </div>
      <P>
        Você não tem conta?
        <span>
          <router-link to="/registrar">crie uma conta</router-link>
        </span>
      </P>
    </Root>
  </div>
</template>

<script>
import "lume/dist/lib/lume.css";
import { Root, H1, P, Button, Input} from "lume";

export default {
  components: {
    Root,
    H1,
    P,
    Button,
    Input
  },
  name: "vue-login",
  data() {
    return {};
  },
  methods: {
    login: function () {
      this.$router.replace("/");
    },
  },
};
</script>

<style lang="scss" scoped>
.login {
  margin-top: 40px;
}
input {
  margin: 10px 0;
  width: 20%;
  padding: 15px;
}
button {
  font-family: "Roboto", sans-serif;
  text-transform: uppercase;
  outline: 0;
  background: #4caf50;
  border: 0;
  padding: 15px;
  color: #ffffff;
  font-size: 14px;
  -webkit-transition: all 0.3 ease;
  transition: all 0.3 ease;
  cursor: pointer;
}
p {
  margin-top: 40px;
  font-size: 13px;
}
p a {
  text-decoration: underline;
  cursor: pointer;
}
</style>