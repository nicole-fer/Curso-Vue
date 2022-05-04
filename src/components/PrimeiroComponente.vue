<template>
    <div>
        <h1>Olá Vue</h1>
        <p> Meu nome é {{nome}}, tenho {{age}} anos, sou {{profissao}}</p>
        <MultiplosEventos/>
    </div>
</template>

<script>
import MultiplosEventos from './MultiplosEventos.vue'
    export default {
        name: 'PrimeiroComponente',
        components : {
            MultiplosEventos
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
