<template>
    <div>
        <div class="row mt-3">
            <div class="col-xs-6">
                <h4>Lista de Productos</h4>
                
            </div>
            <div class="col-xs-6 ml-5">
                <b-button variant="primary" href="/productos/nuevo">
                    Nuevo
                </b-button>
            </div>
        </div>

        <div class="row mt-4">
            <div class="col-sm-12">
                <b-table responsive striped hover :fields="fields" />
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data(){
        return{
            fields: [ 'Imagen', 'Nombre', 'Precio', 'Cantidad', 'Acciones' ]
        }
    }
}
</script>

