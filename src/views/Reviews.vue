<template>
<div class="reviews">
    <v-container>
        <h2 class="text-h6 font-weight-bold">Client Reviews</h2>
        <v-row class="d-flex justify-center">
            <v-col cols="12" sm="12" md="10" lg="10" xl="10">
                <TheSwiper  :cards="cards"/>
            </v-col>
        </v-row>
        <!-- <div class="box"  >
          
        </div> -->
    </v-container>
</div>
</template>

<script>
import TheSwiper from '@/components/TheSwiper.vue';

export default {
    name: 'reviews',
    data() {
        return {
            cards: [{
                    id: 1,
                    name: 'Jone',
                    sub: 'subtitle',
                    img:'https://img.lovepik.com/element/40028/0241.png_300.png',
                    text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Harum nihil numquam rerum  '
                },
                {
                    id: 2,
                    name: 'name',
                    sub: 'subtitle',
                    img:'https://www.pngall.com/wp-content/uploads/8/Young-Man-PNG-Free-Image.png',
                    text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Harum nihil numquam rerum '
                },
                {
                    id: 3,
                    name: 'name',
                    sub: 'subtitle',
                    img:'https://w7.pngwing.com/pngs/229/266/png-transparent-management-consultant-businessperson-idea-project-young-men-and-women-miscellaneous-association-recruiter.png',
                    text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Harum nihil numquam rerum  '
                },
                {
                    id: 4,
                    name: 'name',
                    sub: 'subtitle',
                    img:'https://img.lovepik.com/free-png/20211225/lovepik-young-business-women-png-image_400317477_wh300.png',
                    text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Harum nihil numquam rerum  '
                },
                {
                    id: 5,
                    name: 'name',
                    sub: 'subtitle',
                    img:'https://www.pngmart.com/files/15/Business-Woman-PNG-Photos.png',
                    text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Harum nihil numquam rerum  '
                },
                {
                    id: 6,
                    name: 'name',
                    sub: 'subtitle',
                    img:'https://purepng.com/public/uploads/large/purepng.com-manmanadult-malemale-childboy-beingmens-1421526920869cscbo.png',
                    text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Harum nihil numquam rerum  '
                },
            ]
        }
    },
    components:{
        TheSwiper
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
    display: flex;
    justify-content: center;
}
</style>
