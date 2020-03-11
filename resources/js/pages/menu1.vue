<template>
    <v-app> 
        <Header/>       
        <v-content>
            <v-container class="fill-height" fluid>
                <v-row aling="center" justify="center">
                    <v-col class="text-center">
                        Hola a todos
                    </v-col>
                </v-row>
            </v-container>
        </v-content>
        <FooterCore/>
    </v-app>
</template>

<script>
import Header from '../components/Header';

    export default {
        components: {
            Header,
            FooterCore: () => import("../components/Footer")
        },
    }
</script>

