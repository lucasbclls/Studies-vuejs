<template>
  <div>
    <p>Meu nome é {{ nome }}</p>
  </div>
</template>


<script>
export default {
  name: "LifeCycle",
  data() {
    return {
      nome: "Ainda não sei",
    };
  },
  created() {
    setTimeout(() => {
      this.nome = "Pedro";
    }, 1000);
  },
  mounted() {
    setTimeout(() => {
      this.nome = "Lucas";
    }, 2000);
  },
};
</script>
