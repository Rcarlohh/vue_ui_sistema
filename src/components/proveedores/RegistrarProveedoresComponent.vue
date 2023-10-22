<template>
    <div class="container">
        <div class="row">
            <div class="col-xs-12 col-sm-12 col-md-8 col-lg-8">
                <template>
                    <v-card class="mx-auto">
                        <v-card-text>
                            <div>Datos Generales</div>
                            <p class="text-h4 text--primary">
                                Nuevo Proveedor
                            </p>
                            <div class="text--primary">
                                <v-form v-model="valid">
                                    <v-container>
                                        <v-row>
                                            <v-col cols="12" md="4">
                                                <v-text-field v-model="RFC" :rules="rfc" :counter="10" label="RFC"
                                                    required hide-details></v-text-field>
                                            </v-col>

                                            <v-col cols="12" md="4">
                                                <v-text-field v-model="lastname" :rules="nameRules" :counter="10"
                                                    label="Razon Social" hide-details required></v-text-field>
                                            </v-col>

                                            <v-col cols="12" md="4">
                                                <v-text-field v-model="contacto" :rules="emailRules" label="Contacto"
                                                    hide-details required></v-text-field>
                                            </v-col>
                                            <v-col cols="12" md="4">
                                                <v-text-field v-model="telefonop" :rules="emailRules" label="Telefono Principal"
                                                    hide-details required></v-text-field>
                                            </v-col>
                                            <v-col cols="12" md="4">
                                                <v-text-field v-model="telefonom" :rules="emailRules" label="Telefono Movil"
                                                    hide-details required></v-text-field>
                                            </v-col>
                                            <v-col cols="12" md="4">
                                                <v-text-field v-model="estado" :rules="emailRules" label="Estado" hide-details
                                                    required></v-text-field>
                                            </v-col>
                                            <v-col cols="12" md="4">
                                                <v-text-field v-model="email" :rules="emailRules" label="EMAIL" hide-details
                                                    required></v-text-field>
                                            </v-col>
                                        </v-row>
                                    </v-container><br>
                                    <p>Direccion</p>
                                    <v-form v-model="valid">
                                        <v-container>
                                            <v-row>
                                                <v-col cols="12" md="4">
                                                    <v-text-field v-model="cp" :rules="yes" label="Codigo Postal"
                                                        hide-details required></v-text-field>
                                                </v-col>
                                                <v-col cols="12" md="4">
                                                    <v-text-field v-model="numeros" :rules="yes"
                                                        label="Numero Interior" hide-details required></v-text-field>
                                                </v-col>
                                                <v-col cols="12" md="4">
                                                    <v-text-field v-model="numeros" :rules="yes"
                                                        label="Numeor Exterior" hide-details required></v-text-field>
                                                </v-col>
                                                <v-col cols="12" md="4">
                                                    <v-text-field v-model="calle" :rules="yes" label="Calle"
                                                        hide-details required></v-text-field>
                                                </v-col>
                                                <v-col cols="12" md="4">
                                                    <v-text-field v-model="Colonia" :rules="yes" label="Colonia"
                                                        hide-details required></v-text-field>
                                                </v-col>
                                                <v-col cols="12" md="4">
                                                    <v-text-field v-model="Entidad" :rules="yes" label="Entidad"
                                                        hide-details required></v-text-field>
                                                </v-col>
                                                <v-col cols="12" md="4">
                                                    <v-text-field v-model="Municipio" :rules="yes" label="Municipio"
                                                        hide-details required></v-text-field>
                                                </v-col>
                                            </v-row>
                                        </v-container>
                                    </v-form>
                                </v-form>
                            </div>
                        </v-card-text>
                        <v-card-actions>
                            <v-btn variant="text" color="teal-accent-4" @click="reveal = true">
                                Guardar
                            </v-btn>
                        </v-card-actions>

                        <v-expand-transition>
                            <v-card v-if="reveal" class="v-card--reveal" style="height: 100%;">
                                <v-card-text class="pb-0">
                                    <p class="text-h4 text--primary">
                                        Origin
                                    </p>
                                    <p>late 16th century (as a noun denoting a place where alms were distributed): from
                                        medieval Latin eleemosynarius, from late Latin eleemosyna ‘alms’, from Greek
                                        eleēmosunē ‘compassion’ </p>
                                </v-card-text>
                                <v-card-actions class="pt-0">
                                    <v-btn variant="text" color="teal-accent-4" @click="reveal = false">
                                        Close
                                    </v-btn>
                                </v-card-actions>
                            </v-card>
                        </v-expand-transition>
                    </v-card>
                </template>
            </div>
                <div class="col-xs-12 col-sm-12 col-md-4 col-lg-4">
                    <template>
                        <v-card class="mx-auto" max-width="344">
                            <v-card-text>
                                <p class="text-h4 text--primary">
                                    Detalle del Proveedor</p>
                                   <div class="text--primary">b
                                    <v-list-item>
                                        <v-list-content>
                                            <v-text-field v-model="RFC" :rules="rfc" label="RFC"
                                                        hide-details required></v-text-field>
                                        </v-list-content>
                                    </v-list-item>

                                </div>
                            </v-card-text>
                            <v-card-actions>
                               
                            </v-card-actions>

                            <v-expand-transition>
                                <v-card v-if="reveal" class="v-card--reveal" style="height: 100%;">
                                    <v-card-text class="pb-0">
                                        <p class="text-h4 text--primary">
                                            Origin
                                        </p>

                                    </v-card-text>
                                    <v-card-actions class="pt-0">
                                        <v-btn variant="text" color="teal-accent-4" @click="reveal = false">
                                            Close
                                        </v-btn>
                                    </v-card-actions>
                                </v-card>
                            </v-expand-transition>
                        </v-card>
                    </template>
                </div>
            
        </div>

    </div>
</template>

<script>
import { required, max, min } from 'vee-validate/dist/rules';
import { extend, ValidationObserver, ValidationProvider } from 'vee/validate';
export default {
    name: 'RegistrarProveedoresComponent',
    data: () => ({
        valid: false,
        firstname: '',
        lastname: '',
        nameRules: [
            value => {
                if (value) return true

                return 'Name is required.'
            },
            value => {
                if (value?.length <= 10) return true

                return 'Name must be less than 10 characters.'
            },
        ],
        email: '',
        emailRules: [
            value => {
                if (value) return true

                return 'E-mail is requred.'
            },
            value => {
                if (/.+@.+\..+/.test(value)) return true

                return 'E-mail must be valid.'
            },
        ],
        
    }),
}


</script>
<style></style>