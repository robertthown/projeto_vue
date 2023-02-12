<template>
    <div>
        <img :src="avatar" :alt="descricao">
        <MudarImagemVue @mudar-imagem="trocarImagem"/>
    </div>
</template>

<script>
import Reutilizacao from './Reutilizacao.vue';
import MudarImagemVue from './MudarImagem.vue';


export default {
    name: "Picture",
    data() {
        return {
            avatar: "../img/avatar.png",
            descricao: "Roberto Melo"
        };
    },
    components: { 
        Reutilizacao, 
        MudarImagemVue
     },
     methods: {
        trocarImagem(){
            this.avatar = "../img/avatar2.png"
        }
     }
}
</script> 