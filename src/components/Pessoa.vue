<template>
    <div>
        <h2>Esta é a descrição da pessoa: {{nome}} </h2>
        <Info :email="email" :esta_trabalhando="true"/>
        <Form/>
    </div>
</template>

<script>
// APP > PESSOA > INFO - HIERARQUIA

import Info from './Info.vue'
import Form from './Form'

    export default {
        name: 'PessoaP',
        components:{
            Info,
            Form
        },
        data(){
            return{
                nome: 'Zezim',
                email: 'nicolefernandes2@gmail.com',
            }
        }
    }
</script>

