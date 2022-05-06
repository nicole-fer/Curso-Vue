<template>
  <div class="main-conteiner">
      <h1>Gerenciar Pedidos: </h1>
      <Dashboards/>
  </div>
</template>

<script>
import Dashboards from '../components/Dashboards.vue'
    export default {
        name: 'PedidosComponent',
        components: {
            Dashboards
        }
    }
</script>

