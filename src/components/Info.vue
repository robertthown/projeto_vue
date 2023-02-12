<template>
    <div>
        <p>{{ email }}</p>
        <p v-show="esta_trabalhando">Estou trabalhando no momento.</p>
        <p>Utilizo as seguintes tecnologias:</p>
        <ul>
            <li>JavaScript</li>
            <li>Vue</li>
            <li>HTML/CSS</li>
        </ul>
        <Picture />
    </div>
</template>

<script>

import Picture from './Picture.vue';

export default {
    name: "Info",
    components: {
        Picture
    },
    props:{
        email: String,
        esta_trabalhando: Boolean
    },
    data(){
        return {
            mostrar_email: false,
            meu_link: 'https://google.com',
            textoBotao: 'Mostrar e-mail',
            backend_technologies: ['Js', 'php', 'python'],
            frontend_technologies: [
                {id: 1, language: 'HTML'},
                {id: 2, language: 'CSS'},
                {id: 3, language: 'VUE'},
            ]
        }
    }
}
</script>