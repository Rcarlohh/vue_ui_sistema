<template>
    <div class="container">
        <div class="row">
            <div class="col-xs-12  col-sm-12 col-md-12 col-lg-12">
                <v-btn
                outlined
                color="indigo"
                class="pa-1 ml-auto ma-1 d-felx align-end flex-column" @click="navigateRegister">
                <v-icon dark>
                    mdi-plus
                </v-icon>
                Agregar-Nuevo</v-btn>
                <v-card
                    class="mx-auto"
                    max-withd="100%"
                    clevation="6"
                    >
                 <v-card-text>
                    <h1 class="letter text-h4 ">Administracion de Proveedores </h1>
                    <p class='letter'>Filtro de Busqueda </p>
                 </v-card-text>
                 <TableComponent></TableComponent>
                </v-card>
            </div>
        </div>
    </div>
</template>
<script>
import HomeView from '@/views/HomeView.vue';
import TableComponent from './TableComponent.vue'

export default {
    name: 'ManagerComponent',
    components: { 
        HomeView,
        TableComponent 
    }, 
   methods: {
        navigateRegister(){
            this.$router.push("/registrar-proveedores");
        }
    }
}
</script>
<style>
    .letter{
    font-family: 'Roboto Slab', serif;
    font-weight: 900;
    }

</style>