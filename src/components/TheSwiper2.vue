<template>
<div ref="swiper" class="swiper">

    <div class="swiper-wrapper">
        <div class="swiper-slide image" v-for="card in cards" :key="card.id" >
            <!-- <div class="image"> -->
                <v-img :src="card.image" class="img"/>
            <!-- </div> -->

        </div>
    </div>
    <!-- <div class="swiper-pagination"></div> -->

    <!-- If we need navigation buttons -->
    <div class="swiper-button-prev"></div>
    <div class="swiper-button-next"></div>

    <!-- If we need scrollbar -->
    <div class="swiper-scrollbar"></div>
</div>
</template>

<script>
import Swiper, {
    Navigation,
    Pagination
} from 'swiper'
import 'swiper/css'
import 'swiper/css/navigation'
import 'swiper/css/pagination'
import ReviewCard from './ReviewCard.vue'
export default {
    props: ['cards'],

    mounted() {
        new Swiper(this.$refs.swiper, {
            // configure Swiper to use modules
            modules: [Navigation, Pagination],
            // Optional parameters
            loop: true,
            slidesPerView: 5,
            spaceBetween: 10,
            // autoplay: {
            //     delay: 500,
            //     disableOnInteraction: false,
            // },

            // If we need pagination
            pagination: {
                el: '.swiper-pagination',
            },

            // Navigation arrows
            navigation: {
                nextEl: '.swiper-button-next',
                prevEl: '.swiper-button-prev',
            },

            // And if we need scrollbar
            scrollbar: {
                el: '.swiper-scrollbar',
            },
        })
    },

    components: {
        ReviewCard
    }
}
</script>

<style scoped>
.swiper-slide {
    display: flex;
    justify-content: center;
    align-items: center;
}

.image {
    display: grid;
    grid-template-rows: repeat(25px,10);
}

.image:nth-child(1) {
    grid-column: 1/2;
    grid-row: 3/8;
    margin-top: 20px;
    margin-bottom:20px;
    /* margin-top: 20px; */
}

.image:nth-child(2) {
    grid-column: 2/3;
    grid-row: 2/9;
    margin-top: 10px;
    margin-bottom:10px;
    /* margin-top: 10px */
}

.image:nth-child(3) {
    grid-column: 3/4;
    grid-row: 1/10;
}

.image:nth-child(4) {
    grid-column: 4/5;
    grid-row: 2/9;
    margin-top: 10px;
    margin-bottom:10px;
    /* margin-top: 10px */
}

.image:nth-child(5) {
    grid-column: 5/6;
    grid-row: 3/8;
    margin-top: 20px;
    margin-bottom:20px;
}

.image .img {
    padding: 5px;
    background-position: center;
    background-size: cover;
    height: 250px;
    border-radius: 10px;

}
</style>
