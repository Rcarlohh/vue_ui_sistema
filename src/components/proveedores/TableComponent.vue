<template>
    <v-data-table
        :headers="headers"
        :items="desserts"
        sort-by="calories"
        class="elevation-1"
    >
    <template v-slot:top>
        <v-toolbar
        flat
        >
            <v-toolbar-title>
                <i class="fas fa-user-circle"></i>
                Proveedores
            </v-toolbar-title>
            <v-divider class="mx-4" inset vertical>
            </v-divider>
            <v-spacer></v-spacer>
            <v-dialog
            v-model="dialog"
            max-widht="500px"
            >
                <template v-slot:activator="{on, attrs}">

                </template>
                <v-card>
                    <v-card-title>
                        <span class="text-h5"> {{ formTitle }}</span>
                    </v-card-title>
                </v-card>
            </v-dialog>
        </v-toolbar>

    </template>
    </v-data-table>
</template>

<script>

export default {

}

</script>