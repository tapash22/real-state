<template>
<div class="the-footer">
    <v-row class="d-flex justify-center green">
        <v-col cols="12" sm="12" md="3" lg="3" xl="3" class="d-flex justify-end">
            <div class="box">
                <h2>name</h2>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Adipisci, illum!</p>
            </div>
        </v-col>

        <v-col cols="12" sm="12" md="2" lg="2" xl="2" class="d-flex justify-center">
            <div class="box">
                <h2>name</h2>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Adipisci, illum!</p>
            </div>
        </v-col>
        <v-col cols="12" sm="12" md="2" lg="2" xl="2" class="d-flex justify-center">
            <div class="box">
                <h2>name</h2>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Adipisci, illum!</p>
            </div>
        </v-col>
         <v-col cols="12" sm="12" md="2" lg="2" xl="2" class="d-flex justify-center">
            <div class="box">
                <h2>name</h2>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Adipisci, illum!</p>
            </div>
        </v-col>

        <v-col cols="12" sm="12" md="3" lg="3" xl="3" class="d-flex justify-center">
            <v-list class="d-block" color="transparent">
                <v-list-item-title class="text-h6">Connecting link</v-list-item-title>
                <v-list-item class="d-flex justify-space-evenly " >
                    <v-avatar size="32" color="red" class="mx-2 my-2" v-for="list in lists" :key="list">
                        <v-icon color="white"  >mdi-{{list}}</v-icon>
                    </v-avatar>
                    
                </v-list-item>
            </v-list>
        </v-col>
    </v-row>
</div>
</template>

<script>
export default {
    name:'the-footer',
    data(){
        return{
             lists:['facebook','linkedin','twitter']
        }
    }
}
</script>

<style scoped>
.box {
    display: block;
    padding: 10px;
    margin: 0;
}

.box h2 {
    font-size: 1em;
    font-weight: 700;
}

.box p {
    font-size: 0.8rem;
    font-weight: 400;
}
</style>
