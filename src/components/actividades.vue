<template>
  <v-container fluid class="background-contenido height">
    <v-row no-gutters >
      <v-row class="mr-5">
      <!--  <v-col align="center">
          <v-btn :to="{ name: 'decimal' }" color="indigo" class="btn_background mx-5" block outlined dark rounded x-large>
            
            <h1>decimal</h1>
          </v-btn>
        </v-col> -->
        <v-col align="center">
          <v-btn :to="{ name: 'act1' }" color="pink"  class="btn_background mx-5" block outlined dark rounded x-large>
            <!-- <v-icon class="my-n ml-n3" size="50"> mdi-gamepad-round-up </v-icon> -->
            <h1>Actividad 1</h1>
          </v-btn>
        </v-col>
        <!--  -->

         <v-col align="center">
          <v-btn :to="{ name: 'act2' }" color="blue"  class="btn_background mx-5" block outlined dark rounded x-large>
            <!-- <v-icon class="my-n ml-n3" size="50"> mdi-gamepad-round-up </v-icon> -->
            <h1>Actividad 2</h1>
          </v-btn>
        </v-col>
      </v-row>
    </v-row>
    <v-row no-gutters>
      <v-col align="center">
        <v-main style="padding: 10px 0px 0px">
              <transition name="bounce">
                <router-view></router-view>
              </transition>
        </v-main>
      </v-col>
    </v-row>
  </v-container>
</template>

<style>
.btn_background{
  background-color: rgba(0, 0, 0, 0.5); 
   /* border-bottom:4px solid rgb(255, 255, 255) ; */
}
</style>

<script>
export default {
  name: "Actividades",
  data: () => ({
    //
  }),

  beforeDestroy() {
  },
};
</script>
