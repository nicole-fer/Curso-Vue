<template>
    <div>
        <Reutilizacao/>
        <h1>Olá Vue</h1>
        <p> Meu nome é {{nome}}, tenho {{age}} anos, sou {{profissao}}</p>
        <Reutilizacao/>
        <MultiplosEventos/>
        <Reutilizacao/>
        <Reutilizacao/>
        <Reutilizacao/>
        <Reutilizacao/>
        <Reutilizacao/>
    </div>
</template>

<script>
import MultiplosEventos from './MultiplosEventos.vue'
import Reutilizacao from './Reutilizacao.vue'

    export default {
        name: 'PrimeiroComponente',
        components : {
            MultiplosEventos,
            Reutilizacao
        },
        data(){
            return {
                nome: 'Nicole',
                age: 22,
                profissao: 'programadora'
            }
        }
    }
</script>
