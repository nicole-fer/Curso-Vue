<template>
    <ul>
        <li>
            <a href="#"> Home</a>
        </li>

        <li>
            <a href="#"> Projetos</a>
        </li>

        <li>
            <a href="#"> Contatos</a>
        </li>

        <li>
            <a v-if="esta_logado" href="#"> Meu Perfil</a>
        </li>
    </ul>
</template>

<script>
    export default {
        name:'HeadeR',
        props: ["esta_logado"]
    }
</script>

<style scoped>
    ul{
        list-style: none;
        display: flex;
        background: white;
    }
    li {
        margin-right: 10px;
        font-size: 22px;
    }
    a {
        color: rgb(12, 97, 171);
        text-decoration: none;
        transition: .5s;
    }
    a:hover{
        color: turquoise;
    }
</style>