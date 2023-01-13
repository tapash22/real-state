<template>
    <div class="the-navigation">
        <v-app-bar elevation="0" color="white">
            <v-app-bar-nav-icon class="hidden-md-and-up"/>
            <v-app-bar-title class="title">RealState</v-app-bar-title>
            <v-spacer></v-spacer>
            <v-list class="d-flex" v-for='list in lists' :key="list.id" style="background:transparent">
                <router-link :to="list.link" style="text-decoration:none;">
                <v-list-item >
                    {{list.name}}
                </v-list-item>
                </router-link>
            </v-list>
            <v-btn outlined small color="green" class="white--text"> upload</v-btn>
            <v-btn outlined small  color="green" class="white--text mx-2"> Register</v-btn>
        </v-app-bar>
    </div>
</template>

<script>
export default {
    name:'the-navigation',
    data(){
        return{
            lists:[
                {
                    id:1,
                    name:'Home',
                    link:'home'
                },
                {
                    id:2,
                    name:'About',
                    link:'about'
                },
                {
                    id:3,
                    name:'Client',
                    link:'about'
                },
                {
                    id:4,
                    name:'Project',
                    link:'about'
                },
                
            ]
        }
    }
}
</script>


<style scoped>
.title{
    width: 120px;
}
</style>