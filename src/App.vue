<template>
  <div>
  <Header :esta_logado="false" />
  <primeiro-componente />
  <SegundoComponente />
  <p>o Dado de app é: {{testando}}</p>
  <LifeCycle />
  <Pessoa />

  </div>

</template>

<script>

  import PrimeiroComponente from './components/PrimeiroComponente.vue'
  import SegundoComponente from './components/SegundoComponente.vue'
  import LifeCycle from './components/LifeCycle.vue'
  import Pessoa from './components/Pessoa.vue'
  import Header from './components/Header.vue'

  export default{
    name: 'App',
    components: {
      PrimeiroComponente, 
      SegundoComponente, 
      LifeCycle,
      Pessoa, 
      Header
    },
    data(){
      return{
      testando: "teste"
      }
    }
  }

</script>