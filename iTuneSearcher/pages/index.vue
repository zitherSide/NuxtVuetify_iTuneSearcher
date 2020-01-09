<template>
    <div>
        <v-layout align-center column>
            <h1>Search iTunes</h1>
            <br/>

            <v-text-field v-model="search" placeholder="Enter Artist Name" autofocus/>
            <v-card>
                <v-card-title>{{search}}</v-card-title>
            </v-card>
        </v-layout>
    </div>
</template>

<script>
export default{
    data(){
        return{
            search:""
        }
    }
}
</script>
