<template>
  <h2>Meu formulario</h2>
  <form action="" @submit="EnviarFormulario($event)">
    <div>
      <input type="text" v-model="name" />
    </div>

    <div>
      <input type="text" v-model="email" />
    </div>

    <div>
      <input type="submit" />
    </div>
  </form>
</template>
<p>Conteudo!</p>
<p>Conteudo!</p>
<p>Conteudo!</p>
<script>
export default {
  name: "Form",

  data() {
    return {
        name:"",
        email: ""
    }
  },

  methods: {
    EnviarFormulario() {
      e.preventDefault();
      const name = this.name;
      const email = this.email;
      console.log("Formulario Enviado!");
      console.log("O nome é:" + name);
      console.log("O email é:" + email);

      // Ajax

      //Inserir no BD
    },
  },
};
</script>

<style scoped>
p {
  margin: 150px;
}
</style>
