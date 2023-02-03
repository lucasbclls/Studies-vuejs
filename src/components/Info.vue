<template>
  <div>
    <p v-if="esta_trabalhando">
      Estou trabalhando no momento <br />
      Utilizo as seguintes linguagens de programação
    </p>
    <p v-else>Estou em busca de novas oportunidades</p>
    <p>Utilizo as seguintes tecnolgias para back-end:</p>

    <ul>
      <li
        v-for="(technology, index) in backend_technologies"
        v-bind:key="index"
      >
        {{ technology }}
      </li>
    </ul>
    <p>Utilizo as seguintes tecnologias para front-end:</p>

    <ul>
      <li v-for="technology in frontend_technologies" :key="technology.id">
      {{ technology.language }}
      </li>
    </ul>
    <p v-show="mostrar_email">Mande uma mensagem para: {{ email }}</p>
    <p class="teste">
      Para acessar meu portifolio
      <a v-bind:href="meu_link" target="_blank">basta clicar aqui</a>
    </p>
    <Picture />
  </div>
</template>

<script>
import Info from "./Info";
import Picture from "./Picture.vue";

export default {
  name: "Info",
  components: {
    Info,
    Picture,
    data() {
      return {
        esta_trabalhando: false,
        mostrar_email: true,
        email: "plucayg@gmail.com",
        meu_link: "https://google.com",
        backend_technologies: ["JavaScript", "PHP", "C#", "Python"],
        frontend_technologies: [
          { id: 1, language: "Vuejs" },
          { id: 2, language: "React Native" },
          { id: 3, language: "Reactjs" },
        ],
      };
    },
  },
};
</script>