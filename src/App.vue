<template>
  <v-app>
    <TheNavigation />
    <v-main>
      <Home />
      <Project />
      <Approved />
      <Reviews />
      <News />
      <TheFooter />
      <!-- <router-view/> -->
    </v-main>
  </v-app>
</template>

<script>
import TheNavigation from '@/components/TheNavigation.vue';
import Home from '@/views/HomeView.vue';
import Project from '@/views/Project.vue';
import Approved from '@/views/Approved.vue';
import Reviews from '@/views/Reviews.vue';
import News from '@/views/News.vue';
import TheFooter from '@/components/TheFooter.vue'


export default {
  name: 'App',

  data: () => ({
    //
  }),

  components:{
    TheNavigation,
    Home,
    Project,
    Approved,
    Reviews,
    News,
    TheFooter
  }
};
</script>
