<template>
    <div>
        <p v-if="esta_trabalhando"> Estou trabalhando no momento</p>
        <p v-else>Estou em busca de novas oportunidades</p>
        <p>Utilizo as seguintes tecnologias: </p>
        <ul>
            <li>JavaScript</li>
            <li>PHP</li>
            <li>Python</li>
        </ul>
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
                mostrar_email: true,
                email: 'nicolefernandesfm@gmail.com',
                meu_link: 'https://github.com/nicole-fer/Curso-Vue'
            }
        }
    }
</script>
