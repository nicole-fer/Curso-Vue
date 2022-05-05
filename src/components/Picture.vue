<template>
    <img :src="avatar" :alt="descricao">
    <Reutilizacao/>
</template>

<script>
import Reutilizacao from './Reutilizacao'

    export default {
        name: 'PicTure',
        components : {
            Reutilizacao
        },
        data() {
            return{
                avatar: "/img/introduction-to-android-1.png",
                descricao: 'Avatar Android andando de Skate'
            }
        }
    }
</script>
