<template>
  <div class="pb-lg-5" >
    <v-container>
      <v-row>
        <v-col cols="9" lg="9" xs="2">
          <v-row>
            <v-col cols="12">
              <h1 class="font font-weight-bold">Blogs</h1>
              <p class="font font-weight-medium">
                your blood journeys through many steps and tests that ensure our
                blood supply is as possible and <br />
                helps as many people as possible.
              </p>
            </v-col>
          </v-row>

          <v-row>
            <v-col cols="12" lg="4" md="10" align="center">
              <v-card class="pa-3 mx-auto" height="300" max-width="275">
                  <div>
                    <v-img
                      :src="require('~/assets/img/blog2.png')"
                      max-height="110"
                      max-width="100"
                    >
                    </v-img>
                  </div>
                      <h1 class="font font-weight-bold text-sm-left">
                        Blood Journey
                      </h1>
                  <p class="font font-weight-medium text-sm-left">
                        Blood banks play an important role 
                        in the process of collecting blood 
                        and managing. updating donations and 
                        updating available blood types. Raster's 
                        web based BBMS will address the issues.
                      </p>
              </v-card>
            </v-col>

            <v-col cols="12" lg="8" md="12"  align="center">
              <v-card class="pa-3" height="300" max-width="550">
                <v-list-item>
                  <div>
                    <v-img
                      :src="require('~/assets/img/blog2.png')"
                      max-height="350"
                      max-width="120"
                    ></v-img>
                  </div>
                  <v-list-item-content>
                    <v-list-item-title>
                      <h1 class="font font-weight-bold text-sm-left">
                        Experience Of <br />
                        Blood Donation
                      </h1></v-list-item-title
                    >
                    <v-list-item-subtitle>
                      <p class="font font-weight-medium text-sm-left">
                        Maintaining adequdle blood supplies requires the<br />
                        recruitment of a significant number of regular<br />
                        donars. However,research examining the first-hand <br />
                        experience of blood donation from the perspective <br />
                        of regular donors is very limited.<br /></p
                    ></v-list-item-subtitle>
                  </v-list-item-content>
                </v-list-item>
              </v-card>
            </v-col>
          </v-row>

          <v-row>
            <v-col cols="12" lg="6" md="8" align="center">
              <v-card class="ml-9 pa-lg-3" height="200" width="370">
                <v-list-item>
                  <div>
                    <v-img
                      :src="require('~/assets/img/blog4.png')"
                      max-height="100"
                      max-width="100"
                    ></v-img>
                  </div>
                  <v-list-item-content>
                    <v-list-item-title>
                      <h1 class="font font-weight-bold text-sm-left">
                        Donate Blood
                      </h1>
                    </v-list-item-title>
                    <v-list-item-subtitle>
                      <p class="font font-weight-medium text-sm-left">
                        your blood journeys through<br />
                        many steps and tests that <br />
                        ensure our blood supply <br />
                        is as possible and helps <br />
                        as many people as possible.<br /></p
                    ></v-list-item-subtitle>
                  </v-list-item-content>
                </v-list-item>
              </v-card>
            </v-col>

            <v-col cols="12" lg="6" md="8" sm="12" align="center">
              <v-card class="pa-3 mr-6" height="200" width="370">
                <v-list-item>
                  <div>
                    <v-img
                      :src="require('~/assets/img/blog3.png')"
                      max-height="100"
                      max-width="100"
                    >
                    </v-img>
                  </div>
                  <v-list-item-content>
                    <v-list-item-title>
                      <h1 class="font font-weight-bold text-sm-left">
                        Donate Blood
                      </h1>
                    </v-list-item-title>
                    <v-list-item-subtitle>
                      <p class="font font-weight-medium text-sm-left">
                        your blood journeys through<br />
                        many steps and tests that <br />
                        ensure our blood supply <br />
                        is as possible and helps <br />
                        as many people as possible.<br />
                      </p>
                    </v-list-item-subtitle>
                  </v-list-item-content>
                </v-list-item>
              </v-card>
            </v-col>
          </v-row>
        </v-col>

        <v-col class="mt-lg-16" cols="12" lg="3" md="8"  align="center">
          <v-card class="mt-3">
            <v-toolbar color="red" dark>
              <v-toolbar-title class="font-weight-bold ml-13"
                >LATEST NEWS</v-toolbar-title
              >
            </v-toolbar>
            <v-list>
              <v-list-item>
                <v-list-item-avatar>
                  <v-img :src="require('~/assets/img/blog2.png')"></v-img>
                </v-list-item-avatar>
                <v-list-item-content>
                  <v-list-item-title class="font-weight-bold text-sm-left">
                    Blood Journey</v-list-item-title
                  >
                  <v-list-item-subtitle class="font-weight-medium text-sm-left">
                    blood banks play an <br />
                    important role in the <br />
                    process of collecting blood.</v-list-item-subtitle
                  >
                </v-list-item-content>
              </v-list-item>

              <v-divider></v-divider>

              <v-list-item>
                <v-list-item-avatar>
                  <v-img :src="require('~/assets/img/blog2.png')"></v-img>
                </v-list-item-avatar>
                <v-list-item-content>
                  <v-list-item-title class="font-weight-bold text-sm-left">
                    Blood Journey</v-list-item-title
                  >
                  <v-list-item-subtitle class="font-weight-medium text-sm-left">
                    blood banks play an <br />
                    important role in the <br />
                    process of collecting blood.</v-list-item-subtitle
                  >
                </v-list-item-content>
              </v-list-item>

              <v-divider></v-divider>

              <v-list-item>
                <v-list-item-avatar>
                  <v-img :src="require('~/assets/img/blog2.png')"></v-img>
                </v-list-item-avatar>
                <v-list-item-content>
                  <v-list-item-title class="font-weight-bold text-sm-left">
                    Blood Journey</v-list-item-title
                  >
                  <v-list-item-subtitle class="font-weight-medium text-sm-left">
                    blood banks play an <br />
                    important role in the <br />
                    process of collecting blood.</v-list-item-subtitle
                  >
                </v-list-item-content>
              </v-list-item>

              <v-divider></v-divider>

              <v-list-item>
                <v-list-item-avatar>
                  <v-img :src="require('~/assets/img/blog2.png')"></v-img>
                </v-list-item-avatar>
                <v-list-item-content>
                  <v-list-item-title class="font-weight-bold text-sm-left">
                    Blood Journey</v-list-item-title
                  >
                  <v-list-item-subtitle class="font-weight-medium text-sm-left">
                    blood banks play an <br />
                    important role in the <br />
                    process of collecting blood.</v-list-item-subtitle
                  >
                </v-list-item-content>
              </v-list-item>

              <v-divider></v-divider>

              <v-list-item>
                <v-list-item-avatar>
                  <v-img :src="require('~/assets/img/blog2.png')"></v-img>
                </v-list-item-avatar>
                <v-list-item-content>
                  <v-list-item-title class="font-weight-bold text-sm-left">
                    Blood Journey</v-list-item-title
                  >
                  <v-list-item-subtitle class="font-weight-medium text-sm-left">
                    blood banks play an <br />
                    important role in the <br />
                    process of collecting blood.</v-list-item-subtitle
                  >
                </v-list-item-content>
              </v-list-item>
            </v-list>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<style>
    .font{
      font-family: Poppins;
    }
</style>
