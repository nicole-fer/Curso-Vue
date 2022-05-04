<template>
    <div id="Form">
        <h2>Meu Formulário</h2>
        <form action="">
            <div>
                <InputText placeholder="Nome"/>
            </div>
            <div>
                <InputText placeholder="E-Mail"/>
            </div>
            <div>
                <Submit/>
            </div>
        </form>
    </div>
</template>

<script>

import InputText from './form/InputText.vue'
import Submit from './form/Submit.vue'

    export default {
        name: 'FormF',
        components:{
            InputText,
            Submit
        }
    }
</script>
