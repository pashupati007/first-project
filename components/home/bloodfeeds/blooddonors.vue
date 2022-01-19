<template>
  <div>
    <v-container>
      <v-card class="ma-10" width="850" height="400">
        <v-row>
          <v-list class="ml-10">
            <v-list-item>
              <v-list-item-avatar>
                <img :src="require('~/assets/img/loginimg/icon2.png')" />
              </v-list-item-avatar>
              <v-list-item-content>
                <v-list-item-title><h2>Blood Donors</h2></v-list-item-title>
                <v-list-item-subtitle></v-list-item-subtitle>
              </v-list-item-content>
            </v-list-item>
          </v-list>

          <v-card class="ml-15 mr-15 mb-5" width="770" height="250"> </v-card>

          <v-row class="ml-15">
            <v-col><v-btn dark color="#DD1F25" width="200">Blog</v-btn></v-col>
            <v-col
              ><v-btn dark color="#DD1F25" width="200">Campaign</v-btn></v-col
            >
            <v-col
              ><v-btn dark color="#DD1F25" width="200"
                >Blood Request</v-btn
              ></v-col
            >
          </v-row>
        </v-row>
      </v-card>
    </v-container>
  </div>
</template>
