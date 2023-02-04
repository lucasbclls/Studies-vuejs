<template>
  <div>
    <Header />
    <PrimeiroComponente />
    <p>O dado de app é {{ testando }}</p>
    <LifeCycle />
    <PessoaCadastro />
    <Info />
    <Form />
  </div>
</template>


<script>
import PrimeiroComponente from "./components/PrimeiroComponente.vue";
import LifeCycle from "./components/LifeCycle.vue";
import PessoaCadastro from "./components/PessoaCadastro.vue";
import Info from "./components/Info.vue";
import Header from "./components/Header.vue";
import Form from "./components/Form.vue";

export default {
  name: "App",
  components: {
    PrimeiroComponente,
    LifeCycle,
    PessoaCadastro,
    Info,
    Header,
    Form,
  },

  data() {
    return {
      testando: "Teste",
    };
  },
};
</script>


<style>
body {
  background-color: #333;
  color: #fff;
}

a {
  color: red;
}
</style>


