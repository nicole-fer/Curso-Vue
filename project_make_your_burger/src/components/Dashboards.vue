<template>
    <div id="burger-table">
        <div>
            <div id="burger-table-heading">
                <div class="order-id">#:</div>
                <div>Cliente</div>
                <div>Pão</div>
                <div>Carne</div>
                <div>Opcionais</div>
                <div>Ações</div>
            </div>
        </div>
        <div id="burger-table-rows">
            <div class="burger-table-row">
                <div class="order-number">1</div>
                <div>Nome do Cliente</div>
                <div>Pao 1</div>
                <div>Carne 2</div>
                <div>
                    <ul>
                        <li>Salame</li>
                        <li>Tomate</li>
                    </ul>
                
            </div>
            <div>
                <select name="status" class="status">
                <option value="">Selecione os dados do Hamburger</option>
                </select>
                <button class="delete-bnt">Cancelar</button>
                </div>
        </div>

                    <div class="burger-table-row">
                <div class="order-number">1</div>
                <div>Nome do Cliente</div>
                <div>Pao 1</div>
                <div>Carne 2</div>
                <div>
                    <ul>
                        <li>Salame</li>
                        <li>Tomate</li>
                    </ul>
                
            </div>
            <div>
                <select name="status" class="status">
                <option value="">Selecione os dados do Hamburger</option>
                </select>
                <button class="delete-bnt">Cancelar</button>
                </div>
        </div>
    </div>
    </div>
</template>

<script>
    export default {
        name: "DashboardsComponent"
    }
</script>

<style scoped>
    #burger-table{
        max-width: 1200px;
        margin: 0 auto;
    }

    #burger-table-heading,
    #burger-table-rows,
    .burger-table-row{
        display: flex;
        flex-wrap: wrap;
    }

    #burger-table-heading {
        font-weight: bold;
        padding: 12px;
        border-bottom: 3px solid;
    }

    #burger-table-heading div,
    .burger-table-row {
        width: 19%;
    }

    .burger-table-row {
        width: 100%;
        padding: 12px;
        border-bottom: 1px solid #CCC;
    }


    #burger-table-heading .order-id,
    .burger-table-row .order-number {
        width: 5%;
    }

    select {
        
    }

</style>
