<template>
  <div>
    <v-container>
      <v-row>
        <v-col cols="3">
          <v-card>
            <v-list>
              <v-list-item>
                <v-avtar> </v-avtar>
                <v-toolbar-title>Give Blood </v-toolbar-title> <br />
                <v-select solo></v-select>
              </v-list-item>
            </v-list>
          </v-card>
        </v-col>


        <v-cols cols="6">
          <v-row>
            <v-col cols="11" align="center">
              <h1>Blood Donation Campaign</h1>
              <v-img></v-img>
              <p>Give Blood,Save life</p>
              <p>
                Date: <br />
                05 jan - 10 jan 2022<br />
                From wed-Monday
              </p>
              <v-divider vertical class="black"></v-divider>
              <p>
                Time: <br />
                11:30 AM. -2 PM.
              </p>
              <p>
                <span>Organized by:</span>Nepal Red Cross Society ||
                <span>Venue:Civil</span>Hospital,New Baneshwor
              </p>
            </v-col>
            <v-row>
              <v-card>
                <v-avtar></v-avtar>
                <v-select> </v-select>
                <v-select> </v-select>
                <v-select> </v-select>
              </v-card>
            </v-row>
          </v-row>
        </v-cols>


        <v-col cols="3"> </v-col>
      </v-row>
    </v-container>
  </div>
</template>
