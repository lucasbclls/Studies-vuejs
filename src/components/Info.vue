<template>
  <div>
    <p v-if="esta_trabalhando">
      Estou trabalhando no momento <br />
      Utilizo as seguintes linguagens de programação
    </p>
    <p v-else>Estou em busca de novas oportunidades</p>
    <ul>
      <li>JavaScript</li>
      <li>PHP</li>
      <li>C#</li>
      <li>NODEJS</li>
    </ul>
    <p v-show="mostrar_email"> Mande uma mensagem para: {{email}}</p>
    <p>Para acessar meu portifolio <a v-bind:href="meu_link" target="_blank">basta clicar aqui</a></p>
    <Picture />
  </div>
</template>

<script>
import Info from "./Info";
import Picture from "./Picture.vue";

export default {
  name: "Info",
  components: {
    Info, Picture,
    data() {
      return {
        esta_trabalhando: false,
        mostrar_email: true,
        email: "plucayg@gmail.com",
        meu_link: 'https://google.com'
      };
    }
    
  },
};
</script>