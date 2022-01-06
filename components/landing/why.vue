<template>
  <div class="pa-10" :height="height" :width="width">
    <v-card class="b pb-10">
      <v-container>
        <v-row>
          <v-col cols="12" class="text-center pt-10">
            <h1 class="font pt-lg-5 font-weight-bold">Why we need?</h1>
            <p class="font pt-lg-5 font-weight-medium">
              Blood banks plau an imporant role inthe process of collecting
              vlood and managing blood stocks, <br />
              approving blood requests upditing donationd and updating available
              blood types.
            </p>
          </v-col>

          <v-col>
            <v-row>
              <v-col cols="12" lg="4" md="6" align="center">
                <div>
                  <v-card class="brd" height="400" width="390">
                    <v-img
                      class="mt-15"
                      :src="require('~/assets/img/icon1.png')"
                      width="100"
                    ></v-img>
                    <h1 class="font font-weight-bold mt-10">Digitalization</h1>
                    <li class="font font-weight-medium">
                      We digitize blood banks.
                    </li>
                    <li class="font font-weight-medium">
                      We digitize blood banks.
                    </li>
                  </v-card>
                </div>
              </v-col>

              <v-col cols="12" lg="4" md="6" align="center">
                <div>
                  <v-card class="brd" height="400" width="390">
                    <v-img
                      class="mt-15"
                      :src="require('~/assets/img/icon2.png')"
                      width="100"
                    >
                    </v-img>
                    <h1 class="font font-weight-bold mt-10">Motivate Donars</h1>
                    <li class="font font-weight-medium">
                      We motivate and retain donors <br />
                      with our vein-to-vein initiative.
                    </li>
                    <li class="font font-weight-medium">
                      We motivate and retain donors <br />
                      with our vein-to-vein initiative.
                    </li>
                  </v-card>
                </div>
              </v-col>

              <v-col cols="12" lg="4" md="12" align="center">
                <div>
                  <v-card class="brd" height="400" width="390">
                    <v-img
                      class="mt-15"
                      :src="require('~/assets/img/icon3.png')"
                      width="100"
                    >
                    </v-img>
                    <h1 class="font-weight-bold mt-10">
                      Ragat chahiyo <br />
                      Hotline
                    </h1>
                    <li class="font font-weight-medium">
                      For emergencies, please call our <br />
                      blood hotline 9825783377.
                    </li>
                    <li class="font font-weight-medium">
                      Working to eliminate blood <br />
                      scarcity in Nepal.
                    </li>
                  </v-card>
                </div>
              </v-col>
            </v-row>
          </v-col>
        </v-row>
      </v-container>
    </v-card>
  </div>
</template>
<style lang="css">
.brd {
  border: 1px solid #ccc !important;
  border-radius: 30px 0 !important;
}

.font {
  font-family: poppins;
}

/* .b {
  border: 1px solid #ccc !important;
  border-radius: 50px 0 !important;
} */
</style>
