<template>
<div class="approved">
    <h2>Proudly Underwritten By</h2>
    <div class="box" >
        <div class="card" v-for="card in cards" :key="card.id" >
            <img :src="card.img" />
        </div>
    </div>
</div>
</template>

<script>
export default {
    name: 'approved',
    data() {
        return {
            cards: [{
                    id: 1,
                    name: 'card1',
                    img: 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSe4b8aIE7CMPCq8OMP933-HoyMQahOKvitaVNIZRUpXuPc8_LcASrdUMsrTqcAzA7cDbY&usqp=CAU'
                },
                {
                    id: 2,
                    name: 'card2',
                    img: 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSe4b8aIE7CMPCq8OMP933-HoyMQahOKvitaVNIZRUpXuPc8_LcASrdUMsrTqcAzA7cDbY&usqp=CAU'
                },
                {
                    id: 3,
                    name: 'card3',
                    img: 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSe4b8aIE7CMPCq8OMP933-HoyMQahOKvitaVNIZRUpXuPc8_LcASrdUMsrTqcAzA7cDbY&usqp=CAU'
                },
                {
                    id: 4,
                    name: 'card4',
                    img: 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSe4b8aIE7CMPCq8OMP933-HoyMQahOKvitaVNIZRUpXuPc8_LcASrdUMsrTqcAzA7cDbY&usqp=CAU'
                },
            ]
        }
    }
}
</script>

<style scoped>
h2 {
    display: flex;
    justify-content: center;
    font-size: 2rem;
    font-weight: 700;
    padding: 20px;
}

.box {
    background: rgba(215, 215, 215,0.5);
    opacity: 0.7;
    display: flex;
    justify-content: center;
    padding:10px;
}
.box .card{
    padding: 10px;

}
.box .card img{
    border-radius: 10%;
    width: 150px;
    height: 100px;
        border: 2px solid greenyellow;
        box-shadow:  0 0 10px greenyellow;
}
</style>
