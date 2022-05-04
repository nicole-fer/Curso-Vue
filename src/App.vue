<template>
  <div>
    <PrimeiroComponente />
    <p class="paragrafo-pai"> O dado de app é: {{testando}}</p>
    <LifeCycle/>
    <Pessoa/>
  </div>

</template>

<script>
import PrimeiroComponente from './components/PrimeiroComponente.vue'
import LifeCycle from './components/LifeCycle.vue'
import Pessoa from './components/Pessoa.vue'

export default{
  name:'App',
  components: {
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
    background-color: rgb(75, 75, 75);
    color: bisque;
  }

  a {
    color: rgb(184, 38, 38);
  }
</style>

