<template>
<div class="home">

        <v-row>
            <v-col cols="12" sm="12" md="3" lg="3" xl="3" class="hidden-sm-and-down">
                <div class="box">
                    <h2>Real state</h2>
                    <v-btn class="btn " outlined large color="green">send message</v-btn>
                </div>
            </v-col>
            <v-col cols="10" sm="10" md="8" lg="8" xl="8">
                <TheSlider />
            </v-col>
              <v-col cols="2" sm="2" md="1" lg="1" xl="1" style="display:grid;">
                <div class="list" >
                  <v-icon class="icon" color="green" v-for="list in lists" :key="list">mdi-{{list}}</v-icon>
                </div>
            </v-col>
        </v-row>
        <!-- <div class="box">
            <div class="text text1">
                1
            </div>
            <div class="text text2">
                2
            </div>
            <div class="text text3">
                3
            </div>
            <div class="text text4">
                4
            </div>
            <div class="text text5">
                5
            </div>
            <div class="text text6">
                6
            </div>
        </div> -->
 
</div>
</template>

<script>
import TheSlider from '@/components/TheSlider.vue';

export default {
    name: 'Home',

    data(){
      return{
        lists:['facebook','linkedin','twitter']
      }
    },

    components: {
        TheSlider
    },
}
</script>

<style scoped>
.box {
    display: grid;
    grid-gap: 1em;
    height: 300px;
}

.box h2 {
    grid-row: 3/4;
    justify-self: center;
    align-self: flex-end;
    font-size: 2rem;
    font-weight: 700;
}

.box .btn {
    grid-row: 4/5;
    align-self: flex-start;
    justify-self: center;
}
.list{
  display: grid;
  grid-gap: 1em;
  align-self: center;
}
.list .icon{

justify-self: start;
align-self: flex-end;
}
/* .list .icon{ */
  /* align-self: flex-start;
  justify-self: end; */
/* } */
</style>
