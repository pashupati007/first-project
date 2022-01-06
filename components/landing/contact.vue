<template>
  <div class="background">
    <v-row>
      <v-col cols="2" class="mt-lg-16 pt-lg-16">
        <v-img :src="require('~/assets/img/bottle.png')"></v-img>
      </v-col>


      <v-col cols="10" algin="center">
        <v-img
          :src="require('~/assets/img/contactback.png')"
          max-width="1270"
          max-height="600"
          class="mt-n3 mb-lg-8"
        >
          <v-row class="mt-lg-10 pt-lg-5">
            <v-col align="center">
              <h1 class="h1blood mb-lg-n5">रागत चहियो ?</h1>
              <br />
              <p class="wrap">
                Fill in the form and send us your details.<br />
                Someone will get back to you if it's an <br />
                emergency.
              </p>
            </v-col>
          </v-row>

          <v-row class="mt-10" justify="center">
            <v-btn color="white" class="mr-5 pa-lg-5" outlined> Request Blood </v-btn>

            <v-btn color="white" class="ml-5 pa-lg-5" outlined> Donate Blood Now</v-btn>
          </v-row>

          <v-row class="mt-10 ml-16 pl-16 pt-10">
            <v-col cols="3 mt-16">
              <v-list-item class="space">
                <v-list-item-content>
                  <v-list-item-title class="font-weight-bold text-sm-left">
                    Contact info
                  </v-list-item-title>
                  <v-list-item-subtitle class="font-weight-medium text-sm-left">
                    Address: Santinagar-05, <br />
                    Kathmandu,Nepal <br />
                    Phone:9825783377 <br />
                    Email: xyzcompany@gmail.com <br />
                  </v-list-item-subtitle>
                </v-list-item-content>
              </v-list-item>
            </v-col>

            <v-col cols="3 mt-16">
              <v-list-item class="space">
                <v-list-item-content>
                  <v-list-item-title class="font-weight-bold text-sm-left">
                    Resources</v-list-item-title
                  >
                  <v-list-item-subtitle class="font-weight-medium text-sm-left">
                    Blood basics <br />
                    Blood bank information <br />
                    When you need blood <br />
                    When you need blood <br />
                    Reports <br />
                    Videos <br />
                    Media Kit <br />
                  </v-list-item-subtitle>
                </v-list-item-content>
              </v-list-item>
            </v-col>

            <v-col cols="3 mt-16">
              <v-list-item class="space">
                <v-list-item-content>
                  <v-list-item-title class="font-weight-bold text-sm-left">
                    Newsletter
                  </v-list-item-title>
                  <v-list-item-subtitle class="font-weight-medium text-sm-left">
                    Subscribe to our <br />
                    Newsletter and get the <br />
                    latest updates about<br />
                    Blood Donation. <br />
                  </v-list-item-subtitle>
                </v-list-item-content>
              </v-list-item>
            </v-col>

            <v-col cols="2 mt-16" align="center">
              <div class="mt-10">
                <v-icon color="blue" class="pa-1">mdi-facebook</v-icon>
                <v-icon class="pa-1">mdi-twitter</v-icon>
                <v-icon color="blue" class="pa-1">mdi-linkedin</v-icon>
                <v-icon class="pa-1">mdi-instagram</v-icon>
              </div>
            </v-col>
          </v-row>
        </v-img>
      </v-col>
    </v-row>


    <v-footer class="background mt-lg-16">
      <hr />
      <p class="pl-10 mb-0">
        Copyright 2022 Donation Group of Companies | All rights reserved |
        Privacy Policy
      </p>
    </v-footer>
  </div>
</template>

<style>
.background {
  background-color: white !important;
}
.space {
  line-height: 10px !important;
}
.h1blood {
  color: white !important;
}
.wrap {
  white-space: wrap;
}
</style>
