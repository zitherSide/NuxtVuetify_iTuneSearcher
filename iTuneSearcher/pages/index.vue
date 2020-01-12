<template>
    <div>
        <v-layout align-center column>
            <h1>Search iTunes</h1>
            <br/>

            <v-row>
                <v-form @submit.prevent="submit">
                    <v-text-field 
                        v-model="search" 
                        label="Enter Artist Name"
                        autofocus/>
                </v-form>
                <v-icon @click="submit">mdi-magnify</v-icon>
            </v-row>
        </v-layout>
    </div>
</template>

<script>
export default{
    data(){
        return{
            search:""
        }
    },
    methods:{
        submit(){
            this.$router.push(`results/${this.search}`)
        }
    }
}
</script>
