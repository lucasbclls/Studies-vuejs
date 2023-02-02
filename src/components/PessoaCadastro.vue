<template>
  <div>
    <h2>Está é a descrição da pessoa: {{ nome }}</h2>
  </div>
</template>

<script>
export default {
  name: "PessoaCadastro",
  data() {
    return {
      nome: "João",
    };
  },
};
</script>