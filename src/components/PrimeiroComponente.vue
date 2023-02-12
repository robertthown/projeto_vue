<template>
    <div>
        <h1>Olá vue!</h1>
        <p>Meu nome é : {{nome}} e trabalho como {{ profissao }}</p>
        <MultiplosEventos />
        <Reutilizacao />
        <Reutilizacao />
        <Reutilizacao />
    </div>
</template>

<script>
    import MultiplosEventos from './MultiplosEventos.vue';
    import Reutilizacao from './Reutilizacao.vue';

export default {

    name: 'PrimeiroComponente',
    data(){
        return{
            nome: "Roberto",
            profissao: "programador"
        }
    },
    components: {MultiplosEventos, Reutilizacao}
}
</script>