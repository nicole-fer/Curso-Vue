<template>
    <div>
        <button @click="primeiro(txt1,$event), segundo(txt2,$event), terceiro()" >Ativar Multiplos Eventos</button>
        <p>{{multiplos_eventos}}</p>
    </div>
</template>

<script>
    export default {
        name: 'MultiplosEventos',
        data() {
            return {
                multiplos_eventos: '',
                txt1: 'Primeiro Evento',
                txt2: 'Segundo Evento',
            }
        },
        // ativa dois metodos com apenas um evento, no primeiro, ao clicar no botão, aparece a frase "Primeiro Evento Ativado" e no segundo substitui a primeira fase pela segunda após meio segundo
        methods: {
            primeiro(txt) {
                this.multiplos_eventos= txt
            },
            segundo(txt) {
                setTimeout(() => this.multiplos_eventos = txt,500)
            },
            terceiro() {
                setTimeout(() => this.multiplos_eventos = " ",1500)
            },
        }
    }
</script>

<style scoped>
    div {
        margin: 100px;
    }
</style>


