<template>
  <v-card flat height="200px">
    <v-toolbar dense>
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
    </v-toolbar>
  </v-card>
</template>

<style>
#magnify {
  transform: rotateY(180deg);
}
</style>
