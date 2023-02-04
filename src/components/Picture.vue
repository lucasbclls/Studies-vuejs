<template>
  <div>
    <img :src="avatar" :alt="descricao" />
    <MudarImagem @muudar-imagem="TrocarImagem" />
  </div>
</template>

<script>
import MudarImagem from './MudarImagem.vue';


export default {
  name: "Picture",
  components: {
    MudarImagem
  },
  data() {
    return {
      avatar: "/img/avatar.png",
      descricao: "Paulo Lucas",
    };
  },
  methods: {
    TrocarImagem(){ 
       this.avatar = "/img/avatar2.png"
    }
  }
};
</script>