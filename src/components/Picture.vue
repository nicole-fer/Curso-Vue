<template>
    <img :src="avatar" :alt="descricao">
</template>

<script>
    export default {
        name: 'PicTure',
        data() {
            return{
                avatar: "/img/introduction-to-android-1.png",
                descricao: 'Avatar Android andando de Skate'
            }
        }
    }
</script>
