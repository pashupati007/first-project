
<template>
  <div :height="height" :width="width" class="image mt-lg-16">
    <v-container class="mid">
      <v-row>
        <v-col cols="12" lg="7" md="6">
          <v-row>
            <v-col class="pl-sm-10">
              <h1 class="font text-lg-h4 text-md-h5 pt-10 font-weight-bold">
                About Us
              </h1>
              <p class="font mt-5 font-weight-medium">
                Existing blood management system in nepal is manual, cumbersome
                and inefficient.
              </p>
              <p class="font font-weight-medium">
                Existing blood management system in nepal is matured, cumbersome
                and inefficient. Most blood banks record the information on
                blood collection supply manually in registers.
              </p>
            </v-col>
          </v-row>

          <v-row>
            <v-col align="center">
              <v-card
                outlined
                height="180"
                width="200"
                class="brd1 border mt-10"
              >
                <p class="text-center">
                  <v-icon color="red" class="mt-10">mdi-hand-heart</v-icon>
                </p>
                <p class="font font-weight-medium text-center">
                  Blood Availability Search
                </p>
              </v-card>

              <v-card
                outlined
                height="180"
                width="200"
                class="brd1 border mt-10"
              >
                <p class="text-center">
                  <v-icon class="mt-10">mdi-iv-bag</v-icon>
                </p>
                <p class="font font-weight-medium text-center">
                  Blood Donation Camps
                </p>
              </v-card>
            </v-col>

            <v-col class="mt-16 me-lg-16" align="center">
              <v-card
                outlined
                height="180"
                width="200"
                class="brd1 border mt-16"
              >
                <p class="text-center">
                  <v-icon class="mt-10">mdi-bank</v-icon>
                </p>
                <p class="font font-weight-medium text-center">
                  Blood Bank Directory
                </p>
              </v-card>
            </v-col>
          </v-row>
        </v-col>

        <v-col lg="5" md="6" class="pl-lg-10" align="center">
          <v-row class="mt-lg-16 ml-lg-16" justify="center">
            <v-card class="size rounded-circle pa-1" height="110" width="110">
              <h1 class="head text-center">80%</h1>
              <p class="font font-weight-medium text-center">
                Blood event organaized
              </p>
            </v-card>

            <v-card class="size rounded-circle ml-10 pa-2" height="110" width="110">
              <h1 class="head text-center">90%</h1>
              <p class="font font-weight-medium text-center">
                Total Blood collected
              </p>
            </v-card>
          </v-row>

          <v-row class="ml-lg-16 pt-lg-10" justify="center">
            <v-card class=" size rounded-circle pa-3" height="110" width="110 ">
              <h1 class="head text-center">65%</h1>
              <p class="font font-weight-medium text-center">Life saved</p>
            </v-card>
          </v-row>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<style lang="css">
.image {
  background-size: 425px;
  background-image: url("~/assets/img/side.svg") !important;
  background-image: no-repeat;
  background-position: right center;
  background-color: #eaeaea;
}

.mid {
  background-image: url("~/assets/img/mid.png") !important;
  background-image: no-repeat;
  background-position: 450px 200px;
  background-size: 250px;
}

.brd1 {
  border: 1px solid #ccc !important;
  border-radius: 10px 20px !important;
}

.head {
  color: #c71c1e;
}
.font{
  font-family: poppins;
}
.size{
  font-size: 13px;
}
</style>

<script>
export default {
  data() {
    return {
      width: 0,
      height: 0,
    };
  },
  mounted() {
    this.height = window.innerHeight;
    this.width = window.innerWidth;
  },
};
</script>
