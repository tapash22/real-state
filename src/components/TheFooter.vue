<template>
<div class="the-footer">
    <v-row class="d-flex justify-center">
        <v-col cols="12" sm="12" md="3" lg="3" xl="3" class="d-flex justify-center">
            <div class="box">
                <h2>name</h2>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Adipisci, illum!</p>
            </div>
        </v-col>
        <v-col cols="12" sm="12" md="3" lg="3" xl="3">
            <div class="box">
                <h2>name</h2>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Adipisci, illum!</p>
            </div>
        </v-col>
        <v-col cols="12" sm="12" md="3" lg="3" xl="3">
            <div class="box">
                <h2>name</h2>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Adipisci, illum!</p>
            </div>
        </v-col>
        <v-col cols="12" sm="12" md="3" lg="3" xl="3">
            <v-list class="d-block">
                <v-list-item-title class="text-h6">link</v-list-item-title>
                <v-list-item class="d-flex justify-space-evenly ">
                    <v-icon color="green">mdi-facebook</v-icon>
                    <v-icon color="green">mdi-facebook</v-icon>
                    <v-icon color="green">mdi-facebook</v-icon>
                </v-list-item>
            </v-list>
        </v-col>
    </v-row>
</div>
</template>

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
