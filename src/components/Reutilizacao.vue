<template>
    <div>
        <button @click="ativar">Clique aqui</button>
        <span v-show="ativou"> Ativado! </span>
    </div>
</template>

<script>
    export default {
        name: 'ReutilizacaoComponente',
        data () {
            return {
                ativou: false   //span fica oculto no começo
            }
        },
        methods: {
            ativar (){
                this.ativou = !this.ativou
            }
        }
    }

</script>



<style scoped>

</style>