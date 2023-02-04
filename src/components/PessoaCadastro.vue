<template>
  <div>
    <h2>Está é a descrição da pessoa: {{ nome }}</h2>
  </div>
  <Form />
  <Info :email = "email"/>
</template>

<script>
import Info from './Info.vue'
import Form from './Form.vue'


export default {
  name: "PessoaCadastro",
   components: {
    Info,Form
   },
  data() {
    return {
      nome: "João",
      email: 'plucasyg@gmail.com'
    };
  },
};
</script>