<template>
    <div>
        <button @click="primeiro(txt1, $event), segundo(txt2, $event), terceiro(txt3, $event)">Ativar múltiplos eventos</button>
        <p>{{ multiplos_eventos }}</p>
    </div>
</template>

<script>
    export default {
        name: 'MultiplosEventos',
        data(){
            return{
                multiplos_eventos: "",
                txt1: "Primeiro evento",
                txt2: "Segundo evento"
            }
        },
        methods: {
            primeiro(txt, e){
                this.multiplos_eventos = txt;
            },
            segundo(txt, e){
                setTimeout(() => this.multiplos_eventos = txt, 1000)
            },
            terceiro(txt3, e){
                setTimeout(() => this.multiplos_eventos = "", 2000)
            }
        }

    }
</script>
<style scoped>
    div {
        margin: 100px;
    }
</style>