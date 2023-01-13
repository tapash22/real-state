<template>
  <v-app>
    <TheNavigation />
    <v-main>
      <Home />
      <Project />
      <!-- <router-view/> -->
    </v-main>
  </v-app>
</template>

<script>
import TheNavigation from '@/components/TheNavigation.vue';
import Home from '@/views/HomeView.vue';
import Project from '@/views/Project.vue';


export default {
  name: 'App',

  data: () => ({
    //
  }),

  components:{
    TheNavigation,
    Home,
    Project,
  }
};
</script>
