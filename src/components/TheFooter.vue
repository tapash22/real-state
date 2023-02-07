<template>
<div class="the-footer">
    <v-row class="d-flex justify-center green">
        <v-col cols="12" sm="12" md="3" lg="3" xl="3" class="d-flex justify-center align-center">
            <div class="box">
                <h1 class="text-h4 font-weight-bold">RealState</h1>
                
            </div>
        </v-col>

        <v-col cols="12" sm="12" md="2" lg="2" xl="2" class="d-flex justify-center">
            <div class="box">
                <h2 class="text-body-1">name</h2>
                <p class="text-body-2">Lorem ipsum dolor sit amet consectetur adipisicing elit. Adipisci, illum!</p>
            </div>
        </v-col>
        <v-col cols="12" sm="12" md="2" lg="2" xl="2" class="d-flex justify-start">
            <div class="box">
                <h2 class="text-body-1 text-start">name</h2>
                <p class="text-body-2">Lorem ipsum dolor sit amet consectetur adipisicing elit. Adipisci, illum!</p>
            </div>
        </v-col>
         <v-col cols="12" sm="12" md="2" lg="2" xl="2" class="d-flex justify-center">
            <div class="box">
                <h2 class="text-body-1">name</h2>
                <p class="text-body-2">Lorem ipsum dolor sit amet consectetur adipisicing elit. Adipisci, illum!</p>
            </div>
        </v-col>

        <v-col cols="12" sm="12" md="3" lg="3" xl="3" class="d-flex justify-center">
            <v-list class="d-flex justify-center align-center" color="transparent">
                
                <v-list-item class="" >
                    <v-avatar size="32" color="white" class="mx-2 my-2" v-for="list in lists" :key="list">
                        <v-icon color="green"  >mdi-{{list}}</v-icon>
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
/* .box {
    display: block;
    padding: 10px;
    margin: 0;
}


.box h2 {
    font-size: 1em;
    font-weight: 700;
     display: flex;
    justify-content: center;
}

.box p {
    font-size: 0.8rem;
    font-weight: 400;
     display: flex;
    text-align: justify;
} */
</style>
