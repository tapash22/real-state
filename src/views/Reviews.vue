<template>
<div class="reviews">
    <v-container>
        <div class="box">
            <v-card  v-for="card in cards" :key="card.id" elevation="4" class="pa-2 mx-2" rounded="lg" width="250">
                <v-card-text class="pa-0" >
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
                <v-card-text class="pa-2 text-body-2 text-justify">
                    {{card.text}}
                </v-card-text>
            </v-card>
        </div>
    </v-container>
</div>
</template>

<script>
export default {
    name: 'reviews',
    data() {
        return {
            cards: [{
                    id: 1,
                    name: 'name',
                    sub: 'subtitle',
                    text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Harum nihil numquam rerum omnis perspiciatis assumenda doloribus quod tempore officiis. Dolor laudantium fugiat architecto aperiam eaque adipisci. Magnam porro eveniet corporis!'
                },
                {
                    id: 2,
                    name: 'name',
                    sub: 'subtitle',
                    text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Harum nihil numquam rerum omnis perspiciatis assumenda doloribus quod tempore officiis. Dolor laudantium fugiat architecto aperiam eaque adipisci. Magnam porro eveniet corporis!'
                },
                {
                    id: 3,
                    name: 'name',
                    sub: 'subtitle',
                    text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Harum nihil numquam rerum omnis perspiciatis assumenda doloribus quod tempore officiis. Dolor laudantium fugiat architecto aperiam eaque adipisci. Magnam porro eveniet corporis!'
                },
            ]
        }
    }
}
</script>

<style scoped>
.box {
    display: flex;
    justify-content: center;
}
</style>
