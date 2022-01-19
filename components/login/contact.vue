<template>
  <div class="background ">
    <v-row>
      <v-col cols="2" class="mt-16 pt-16 hidden-sm-and-down">
        <v-img :src="require('~/assets/img/loginimg/bottle.png')"></v-img>
      </v-col>

      <v-col cols="10" algin="center">
        <v-img
          :src="require('~/assets/img/loginimg/contactback.png')"
          max-width="1270"
          max-height="600"
          class="mt-n3 mb-16"
        >
          <v-row class="mt-10 pt-lg-5 ml-lg-n16" justify="center">
              <h1 class="h1blood">रागत चहियो ?</h1>
          </v-row>
          <v-row justify="center">
              <p class="font wrap">
                Fill in the form and send us your details.<br />
                Someone will get back to you if it's an <br />
                emergency.
              </p>
          </v-row>

          <v-row class="mt-10" justify="center">
            <v-btn color="white" class="mr-5 pa-lg-5" outlined>
              Request Blood
            </v-btn>

            <v-btn color="white" class="ml-5 pa-lg-5" outlined>
              Donate Blood Now</v-btn
            >
          </v-row>

          <v-row class="mt-lg-10 ml-lg-16 pl-lg-16">
            <v-col cols="3" class="mt-lg-16">
              <v-list-item>
                <v-list-item-content>
                  <h1 class="font font-weight-bold text-sm-left">
                    Contact info
                  </h1>
                  <p class="font space font-weight-medium text-sm-left">
                    Address: Santinagar-05, <br />
                    Kathmandu,Nepal <br />
                    Phone:9825783377 <br />
                    Email: xyzcompany@gmail.com <br />
                  </p>
                </v-list-item-content>
              </v-list-item>
            </v-col>

            <v-col cols="3 mt-lg-16">
              <v-list-item>
                <v-list-item-content>
                  <h1 class="font font-weight-bold text-sm-left">
                    Resources
                  </h1>
                  <p class="space font font-weight-medium text-sm-left">
                    Blood basics <br />
                    Blood bank information <br />
                    When you need blood <br />
                    When you need blood <br />
                    Reports <br />
                    Videos <br />
                    Media Kit <br />
                  </p>
                </v-list-item-content>
              </v-list-item>
            </v-col>

            <v-col cols="3 mt-lg-16">
              <v-list-item>
                <v-list-item-content>
                  <h1 class="font font-weight-bold text-sm-left">
                    Newsletter
                  </h1>
                  <p class="space font font-weight-medium text-sm-left">
                    Subscribe to our <br />
                    Newsletter and get the <br />
                    latest updates about<br />
                    Blood Donation. <br />
                  </p>
                </v-list-item-content>
              </v-list-item>
            </v-col>

            <v-col cols="2 mt-lg-16" align="center">
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
    <v-divider class="mt-16 mb-lg-n16"></v-divider>
    <v-footer class="background mt-lg-16">
      <p class="font pl-lg-10 mb-lg-0">
        Copyright © 2022 Donation Group of Companies | All rights reserved |
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
  line-height: 20px !important;
}
.h1blood {
  color: white !important;
  font-size: 40px !important;
}
.wrap {
  white-space: wrap;
  margin-left: 480px;
}
.font {
  font-family: 'Poppins' ,sans-serif;
}
</style>
