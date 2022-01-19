<template>
  <div>
    <v-container>
      <v-card class="ma-10" width="850" height="650">
        <v-row>
          <v-col>
            <v-row>
              <h2 class="post2head ml-16 mt-15 mr-4 font-weight-medium">
                Give Blood, <br />
                Sabe Life!
              </h2>

              <v-divider class="mt-15" inset vertical color="red"></v-divider>

              <h1 class="post2head ml-4 mt-14 font-weight-bold">
                Blood Donation <br />
                Campaign
              </h1>
            </v-row>

            <v-row class="mt-16" justify="center">
              <div class="mt-16">
                <h1>Date:</h1>
                <p>
                  05 jan-10 jan 2022<br />
                  fron wed-Monday
                </p>
              </div>

              <v-img
                :src="require('~/assets/img/homeimg/blooddrop.png')"
                max-height="200"
                max-width="200"
                class="ml-16 mt-5"
              ></v-img>

              <div class="ml-16 mt-16">
                <h1>Time:</h1>
                <p>11:30 AM.-2PM.</p>
              </div>

              <!-- <v-list>
                        <v-list-item>
                            <v-list-item-content>
                                <v-list-item-title>
                                    Date:
                                </v-list-item-title>
                                <v-list-item-subtitle>
                                    05 jan-10 jan 2022
                                </v-list-item-subtitle>
                                <v-list-item-subtitle>
                                    fron wed-Monday
                                </v-list-item-subtitle>
                            </v-list-item-content>
                        </v-list-item>
                    </v-list>

                    <v-img :src="require('~/assets/img/homeimg/blooddrop.png')"></v-img>

                    <v-list>
                        <v-list-item>
                            <v-list-item-content>
                                <v-list-item-title>
                                    Date:
                                </v-list-item-title>
                                <v-list-item-subtitle>
                                    05 jan-10 jan 2022
                                </v-list-item-subtitle>
                                <v-list-item-subtitle>
                                    fron wed-Monday
                                </v-list-item-subtitle>
                            </v-list-item-content>
                        </v-list-item>
                    </v-list> -->
            </v-row>
            <v-row class="mt-16" justify="center">
              <v-card
                class="pa-5"
                width="750"
                height="100"
                color="rgba(241, 12, 5, 0.3)"
              >
                <p><span class="font-weight-bold">Organized by: </span>Nepal Red Cross Society</p>
                <p class="ml-10 mt-n3">
                  <span class="font-weight-bold">Venue: </span> Civil Hospital,New Baneshwor
                </p>
              </v-card>
            </v-row>
          </v-col>
        </v-row>
      </v-card>
    </v-container>
  </div>
</template>

<style>
.post2head{
    color: #DD1F25;
}
</style>