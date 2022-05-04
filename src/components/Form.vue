<template>
    <div id="Form">
        <h2>Meu Formulário</h2>
        <form action="" @submit="EnviarFormulario($event)" >
            <div>
                <input type="text" v-model="name">
            </div>
            <div>
                <input type="text" v-model="email">
            </div>
            <div>
                <Submit/>
            </div>
        </form>
        <p>Conteúdo</p>
        <p>Conteúdo</p>
        <p>Conteúdo</p>
    </div>
</template>

<script>

//import InputText from './form/InputText.vue'
import Submit from './form/Submit.vue'

    export default {
        name: 'FormF',
        components:{
            Submit,
        },
        data (){
            return {
                name:'',
                email:''
            }
        },
        methods: {
            EnviarFormulario(e) {
                e.preventDefault()

                const name = this.name
                const email = this.email

                console.log("Formulario Enviado!")
                console.log(`O nome é ${name} e o email é ${email}`)

                //Ajax
                //Inserir no banco de dados
            }
        }
    }
</script>

<style scoped>
    p {
        margin: 150px
    }
</style>
