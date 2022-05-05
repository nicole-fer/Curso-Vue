<template>
  <div>
    <Header :esta_logado="true"/>
    <PrimeiroComponente />
    <p class="paragrafo-pai"> O dado de app é: {{testando}}</p>
    <LifeCycle/>
    <Pessoa/>
  </div>

</template>

<script>
import Header from './components/Header.vue'
import PrimeiroComponente from './components/PrimeiroComponente.vue'
import LifeCycle from './components/LifeCycle.vue'
import Pessoa from './components/Pessoa.vue'

export default{
  name:'App',
  components: {
    Header,
    PrimeiroComponente,
    LifeCycle,
    Pessoa,
  },
    data(){
      return{
          testando:'teste'
      }
  }
}
</script>

<style>

  body {
    background-color: rgb(15, 15, 15);
    color: bisque;
  }

  a {
    color: rgb(184, 38, 38);
  }
</style>

