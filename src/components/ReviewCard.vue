<template>
<!-- <div class="review-card" style=""> -->
    <v-card elevation="0" class=" my-2"  >
        <v-card-title class="d-flex justify-center pa-0">
            <v-avatar size="100">
                <v-img :src="card.img" class="white" />
            </v-avatar>
        </v-card-title>
        <v-card-text class="pa-0" >
            <v-card-title class="d-flex justify-center text-body-1 font-weight-bold text-uppercase ">
                {{ card.name }}
            </v-card-title>
            <v-card-subtitle class="d-flex justify-center text-body-1 ">
                {{ card.sub }}
            </v-card-subtitle>
        </v-card-text>
        <v-card-text  class="pa-0">
            <p class="text-body-2 text-center pa-0">
                {{card.text}}
            </p>
            
        </v-card-text>
    </v-card>
<!-- </div> -->
</template>

<script>
export default {
    name: "review-card",
    props: ["card"],

}
</script>

<style scoped>
/* .review-card {
    display: flex;
}

@media only screen and (max-width: 600px) {
    .review-card {
    display: block;
}
} */
</style>
