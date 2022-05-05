<template>
    <img :src="avatar" :alt="descricao">
    <MudarImg @mudar-img="trocarImg"/>
</template>

<script>
//import Reutilizacao from './Reutilizacao'

import MudarImg from './MudarImg.vue'

    export default {
        name: 'PicTure',
        components : {
            MudarImg
            //Reutilizacao
        },
        data() {
            return{
                avatar: "/img/introduction-to-android-1.png",
                descricao: 'Avatar Android andando de Skate',
            }
        },
        methods: {
            trocarImg(){
                if (this.avatar == "/img/introduction-to-android-1.png"){
                    this.avatar = "/img/fto.png"
                } else {
                    this.avatar = "/img/introduction-to-android-1.png"
                }
            }
        }
    }
</script>
