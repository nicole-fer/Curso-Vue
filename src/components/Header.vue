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
    </ul>
</template>

<script>
    export default {
        name:'HeadeR'
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