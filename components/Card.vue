<template>
    <div id="e3"
        style="max-width: 600px; margin: auto;"
        class="grey darken-2">
        <v-container fluid
            style="min-height: 0;"
            grid-list-lg>
            <v-layout row wrap>
                <v-flex xs12>
                    <v-card target="_blank" :href="url" :color="color" class="white--text">
                        <v-container fluid>
                            <v-layout row grid-list-lg>
                                <v-flex xs9>
                                    <v-card-title>{{title}}</v-card-title>
                                    <v-card-text>{{artistName}}</v-card-text>
                                </v-flex>
                                <v-flex xs3>
                                    <v-img
                                        :src="image"
                                        height="125px">
                                    </v-img>
                                </v-flex>
                            </v-layout>
                        </v-container>
                    </v-card>
                </v-flex>
            </v-layout>
        </v-container>
    </div>
</template>

<script>
export default {
    props: [
        'title',
        'image',
        'artistName',
        'url',
        'color'
    ],
}
</script>