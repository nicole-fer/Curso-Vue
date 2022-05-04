<template>
    <h2>Esta é a descrição da pessoa: {{nome}} </h2>
    <Info/>
    <Info/> 
</template>

<script>
// APP > PESSOA > INFO - HIERARQUIA

import Info from './Info.vue'

    export default {
        name: 'PessoaP',
        components:{
            Info
        },
        data(){
            return{
                nome: 'Zezim'
            }
        }
    }
</script>

