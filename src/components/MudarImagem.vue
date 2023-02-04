<template>
<div>
    <button @click="$emit('mudarImagem')">trocar imagem de perfil</button>
</div>
</template>

<script>
export default {
    name: 'MudarImagem',
    emits: ['mudarImagem']

}
</script>