<template>
  <v-app-bar dense flat app clipped-left permanent>
    
      <!-- <v-app-bar-nav-icon></v-app-bar-nav-icon> -->

      <v-spacer></v-spacer>
      <v-spacer></v-spacer>

      <v-btn icon>
        <v-icon>mdi-home-outline</v-icon>
      </v-btn>

      <v-btn icon>
        <v-icon>mdi-heart</v-icon>
      </v-btn>

      <v-btn icon>
        <v-icon icon>mdi-bell-outline</v-icon>
      </v-btn>

      <v-btn icon>
        <v-icon id="magnify">mdi-magnify</v-icon>
      </v-btn>
      <v-spacer></v-spacer>
 
  </v-app-bar>
</template>

<style>
#magnify {
  transform: rotateY(180deg);
}
</style>
