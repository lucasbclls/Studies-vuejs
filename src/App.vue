<template>
  <div>
    <PrimeiroComponente />
    <p>O dado de app é {{ testando }}</p>
    <LifeCycle />
    <PessoaCadastro />
    <Info />
    
  </div>
</template>


<script>
import PrimeiroComponente from "./components/PrimeiroComponente.vue";
import LifeCycle from "./components/LifeCycle.vue";
import PessoaCadastro from "./components/PessoaCadastro.vue";
import Info from "./components/Info.vue";

export default {
  name: "App",
  components: { PrimeiroComponente, LifeCycle, PessoaCadastro, Info },

  data() {
    return {
      testando: "Teste",
    };
  },
};
</script>


    