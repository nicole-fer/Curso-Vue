<template>
    <div>
        <h1>Olá Vue</h1>
        <p> Meu nome é {{nome}}, tenho {{age}} anos, sou {{profissao}}</p>
    </div>
</template>

<script>
    export default {
        name: 'PrimeiroComponente',
        data(){
            return {
                nome: 'Nicole',
                age: 22,
                profissao: 'programadora'
            }
        }
    }
</script>
