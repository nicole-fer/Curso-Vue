<template>
    <h1> Meu nome é:{{nome}}</h1>
</template>


<script>            // data() < created() < mounted()
    export default{
        name:"LifeCycle",
        data(){
            return{
                nome: 'Ainda não sei'
            }
        },
        // troca o quem tem na variavel depois de 1s 
        created(){
            setTimeout(() => {
                this.nome = 'Nicole'
            }, 1000);
        },
        mounted(){
            setTimeout(() => {
                this.nome='Blah Blah'
            },2000)
        }
    }
</script>
