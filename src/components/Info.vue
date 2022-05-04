<template>
    <div>
        <p v-if="esta_trabalhando"> Estou trabalhando no momento</p>
        <p v-else>Estou em busca de novas oportunidades</p>
        <p>Utilizo as seguintes tecnologias para back-end: </p>
        <ul >
            <li v-for="(technology, index) in backend_technology" v-bind:key="index">{{technology}}</li>
        </ul>
        <p>Utilizao as seguintes tecnologias para front-end</p>
        <ul>
            <li v-for="technology in frontend_technology" :key="technology.id">{{ technology.language }}</li>
        </ul>
        <div>
            <button @click="showEmail">{{textoBotao}}</button>
        </div>
        <p v-show="mostrar_email">Mande uma mensagem para: {{email}}</p>
        <p>Para acessar meu portifólio <a v-bind:href='meu_link' target="_blank">  basta clicar aqui</a></p>
        <Picture/>
    </div>
</template>

<script>
import Picture from './Picture.vue'
    export default {
        name:'InfoF',
        components: {
            Picture
        },
        data() {
            return{
                esta_trabalhando: false,
                mostrar_email: false,
                email: 'nicolefernandesfm@gmail.com',
                meu_link: 'https://github.com/nicole-fer/Curso-Vue',
                textoBotao: 'Mostrar E-Mail',
                backend_technology: ['JavaScript','PHP','Python'],
                frontend_technology: [
                    {id: 1 , language: 'HTML'},
                    {id: 2, language: 'CSS'},
                    {id: 3, language: 'Vue'}
                ]
            }
        },
        methods: {
            showEmail(){
                this.mostrar_email = !this.mostrar_email
                if(!this.mostrar_email){
                    this.textoBotao = 'Mostrar E-Mail'
                } else {
                    this.textoBotao = 'Esconder E-Mail'
                }
            }
        }
    }
</script>

<style>
    .paragrafo-pai{
        color: crimson;
    }
</style>
