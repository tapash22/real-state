<template>
<div class="project">
    <v-container>
        <div class="box" >
            <div class="image" v-for="card in cards " :key="card.id">
                <v-img :src="card.image"   class="rounded-lg" />
            </div>
            <!-- <v-card elevation="0">
              
            </v-card> -->
        </div>
    </v-container>
</div>
</template>

<script>
export default {
    name: 'project',
    data() {
        return {
            cards: [{
                    id: 1,
                    image: 'https://images.pexels.com/photos/1133957/pexels-photo-1133957.jpeg?auto=compress&cs=tinysrgb&dpr=1&w=500',
                    name: 'this'
                },
                {
                    id: 2,
                    image: 'https://images.pexels.com/photos/1133957/pexels-photo-1133957.jpeg?auto=compress&cs=tinysrgb&dpr=1&w=500',
                    name: 'this'
                },
                {
                    id: 3,
                    image: 'https://images.pexels.com/photos/1133957/pexels-photo-1133957.jpeg?auto=compress&cs=tinysrgb&dpr=1&w=500',
                    name: 'this'
                },
                {
                    id: 4,
                    image: 'https://images.pexels.com/photos/1133957/pexels-photo-1133957.jpeg?auto=compress&cs=tinysrgb&dpr=1&w=500',
                    name: 'this'
                },
                {
                    id: 5,
                    image: 'https://images.pexels.com/photos/1133957/pexels-photo-1133957.jpeg?auto=compress&cs=tinysrgb&dpr=1&w=500',
                    name: 'this'
                },
            ]
        }
    }
}
</script>

<style scoped>
.box {
    display: grid;
    grid-gap: 5px;
}
.box .image{
    display: grid;
    grid-template-rows: 5;
}
.box .image:nth-child(1){
    grid-column: 1/2;
    grid-row: 1/3;
}
.box .image:nth-child(2){
    grid-column: 2/3;
    grid-row: 3/4;
}
.box .image:nth-child(3){
    grid-column: 3/4;
    grid-row: 4/5;
}
.box .image:nth-child(4){
    grid-column: 4/5;
    grid-row: 3/4;
}
.box .image:nth-child(5){
    grid-column: 5/6;
    grid-row: 1/3;
}
</style>
