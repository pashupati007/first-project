<template>
  <div>
    <v-card class="ml-10 mt-16" width="410" height="580">

      <v-toolbar class="toolbaropacity" dense color="rgba(241, 12, 5, 0.5)">
           <v-spacer></v-spacer>
            <v-toolbar-title>
                <h2>Donar Search</h2>
            </v-toolbar-title>
             <v-spacer></v-spacer>
            <v-app-bar-nav-icon></v-app-bar-nav-icon>
      </v-toolbar>

      <v-list class="ml-10">
        <v-list-item>
          <v-list-content>
            <v-list-item-title>
              <h2>Country</h2>
            </v-list-item-title>
            <v-list-item-subtitle>
              <v-select solo dense label="Select your country"> </v-select>
            </v-list-item-subtitle>
          </v-list-content>
        </v-list-item>

        <v-list-item>
          <v-list-content>
            <v-list-item-title>
              <h2>State</h2>
            </v-list-item-title>
            <v-list-item-subtitle>
              <v-select solo dense label="Select your State"> </v-select>
            </v-list-item-subtitle>
          </v-list-content>
        </v-list-item>

        <v-list-item>
          <v-list-content>
            <v-list-item-title>
              <h2>City</h2>
            </v-list-item-title>
            <v-list-item-subtitle>
              <v-select solo dense label="Select your City"> </v-select>
            </v-list-item-subtitle>
          </v-list-content>
        </v-list-item>

        <v-list-item>
          <v-list-content>
            <v-list-item-title>
              <h2>Area</h2>
            </v-list-item-title>
            <v-list-item-subtitle>
              <v-select solo dense label="Select your Area"> </v-select>
            </v-list-item-subtitle>
          </v-list-content>
        </v-list-item>

        <v-list-item>
          <v-list-content>
            <v-list-item-title>
              <h2>Blood group</h2>
            </v-list-item-title>
            <v-list-item-subtitle>
              <v-select solo dense label="Select your Blood group"> </v-select>
            </v-list-item-subtitle>
          </v-list-content>
        </v-list-item>
      </v-list>

      <div class="text-center">
           <v-btn color="#DD1F25" dark width="300" Elevation>
        <h3>FIND</h3>
      </v-btn>
      </div>
    </v-card>
  </div>
</template>