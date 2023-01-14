<template>
<div class="review-card" style="">
    <v-card v-for="card in cards" :key="card.id" elevation="4" class="pa-2 mx-2 my-2" rounded="lg" width="300">
        <v-card-text class="pa-0">
            <v-list class="d-flex justify-space-around">
                <v-list-item-avatar size="42" color="red" class="d-flex justify-center">
                    <v-img src="@/assets/logo.png" />
                </v-list-item-avatar>
                <v-list-item-content>
                    <v-list-item-title class="text-body-1">{{card.name}}</v-list-item-title>
                    <v-list-item-subtitle class="text-body-2">{{card.sub}}</v-list-item-subtitle>
                </v-list-item-content>
            </v-list>
        </v-card-text>
        <v-card-text class="pa-1 text-body-2 text-justify">
            {{card.text}}
        </v-card-text>
    </v-card>
</div>
</template>

<script>
export default {
    name: 'review-card',
    props: ['cards']
}
</script>

<style scoped>
.review-card {
    display: flex;
}

@media only screen and (max-width: 600px) {
    .review-card {
    display: block;
}
}
</style>
