<template>
  <Banner/>
  <div class="main-conteiner">
    <h1>Monte o Seu Burger:</h1>
    <BurgerForm/>

  </div>
</template>

<script>
import Banner from "../components/Banner.vue"
import BurgerForm from "../components/BurgerForm.vue"

  export default {
    name: 'HommeCompontent',
    components: {
      Banner,
      BurgerForm
    }
  }
</script>
