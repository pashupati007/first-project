<template>
  <div>
    <v-container>
      <v-row>
        <v-col>
          <v-card class="ma-10" width="850" height="430">
            <v-list class="ml-5">
              <v-list-item>
                <v-list-item-avatar>
                  <img :src="require('~/assets/img/loginimg/icon2.png')" alt="" />
                </v-list-item-avatar>
                <v-list-item-content>
                  <v-list-item-title>
                    <h2>Donate Blood</h2>
                  </v-list-item-title>
                  <v-list-item-subtitle>
                    <p>Published on jan 30,2022</p>
                  </v-list-item-subtitle>
                </v-list-item-content>
              </v-list-item>
            </v-list>
            <v-card
              class="ml-15 mr-15 mb-5"
              color="rgba(241, 12, 5, 0.3)"
              width="730"
              height="250"
            >
            </v-card>
            <div class="ml-14">
              <v-icon class="mr-10" size="30">mdi-message-outline</v-icon>

              <v-icon size="40">mdi-share-outline</v-icon>
            </div>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>
