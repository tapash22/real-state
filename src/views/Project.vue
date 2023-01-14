<template>
<div class="project">
    <v-container class="my-2">
        <h2>Blockfox Shorts</h2>
        <div class="box">
            <div class="image" v-for="card in cards " :key="card.id">
                <v-img :src="card.image" class="rounded-xl img" />
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
                    image: 'https://images.unsplash.com/photo-1508450859948-4e04fabaa4ea?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=479&q=80',
                    name: 'this'
                },
                {
                    id: 2,
                    image: 'https://images.unsplash.com/photo-1527335988388-b40ee248d80c?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=387&q=80',
                    name: 'this'
                },
                {
                    id: 3,
                    image: 'https://images.unsplash.com/photo-1508450859948-4e04fabaa4ea?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=479&q=80',
                    name: 'this'
                },
                {
                    id: 4,
                    image: 'https://images.unsplash.com/photo-1429497419816-9ca5cfb4571a?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=871&q=80',
                    name: 'this'
                },
                {
                    id: 5,
                    image: 'https://images.unsplash.com/uploads/14123892966835548e7bd/14369636?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=870&q=80',
                    name: 'this'
                },
            ]
        }
    }
}
</script>

<style scoped>
h2{
    display: flex;
    justify-content: center;
    font-size: 2rem;
    font-weight: 700;
    padding: 20px;
}
.box {
    display: grid;
    grid-template-rows: repeat(20, 10px);
    grid-gap: 5px;
}

.box .image {
    display: grid;
    /* grid-template-rows: 5; */
}

.box .image:nth-child(1) {
    grid-column: 1/2;
    grid-row: 3/18;
    margin-top:20px;
   
}

.box .image:nth-child(2) {
    grid-column: 2/3;
    grid-row: 2/19;
    margin-top:10px
}

.box .image:nth-child(3) {
    grid-column: 3/4;
    grid-row:1/20;
}

.box .image:nth-child(4) {
    grid-column: 4/5;
     grid-row: 2/19;
    margin-top:10px
}

.box .image:nth-child(5) {
    grid-column: 5/6;
   grid-row: 3/18;
    margin-top:20px
}
.box .image .img{
    padding:5px;
    background-position: center;
    background-size: cover;

}
</style>
