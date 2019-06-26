<template>
    <v-flex xs12 sm6 md4 xl3>
        <v-card class="mx-auto" max-width="400" flat>
            <v-divider></v-divider>
            <v-card-title href="#">
                <v-layout row wrap>
                    <v-flex xs12 mb-0 pa-0>
                        <span class="body-2 xs12 mb-0">Roboto</span> <v-icon right color="primary">add_circle</v-icon>
                    </v-flex>
                    <v-flex xs12 pa-0><p class="body-1 font-weight-light mb-0">Twitter</p></v-flex>
                </v-layout>
            </v-card-title>

            <v-card-text class="headline font-weight-bold">
                <v-layout class="options" wrap row>
                    <v-flex xs6 py-0 px-1>
                        <v-select></v-select>
                    </v-flex>
                    <v-flex xs6 py-0 px-1>
                        <v-layout row wrap>
                            <v-flex xs6 class="body-1"><span>33px</span></v-flex>
                            <v-flex xs6 class="body-1"><v-slider></v-slider></v-flex>
                        </v-layout>
                    </v-flex>
                </v-layout>
                <v-textarea v-model="text"></v-textarea>
            </v-card-text>

            <v-card-actions class="pa-0">
                <v-spacer></v-spacer>
                <v-btn small flat>apply to all fonts</v-btn>
                <v-btn small flat>see specimen</v-btn>
            </v-card-actions>
        </v-card>
    </v-flex>
</template>

<script>
export default {

    data() {
        return {
            hovered: false,
            text: "Lorem ipsum"
        }
    }
};
</script>

<style scoped>

    .v-card .v-card__actions {
        display: none;
    }

    .v-card:hover .v-card__actions > *,
    .v-card:hover .v-card__actions {
        display: flex;
    }


</style>
