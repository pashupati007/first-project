<template>
  <div>
    <v-container>
      <v-row>
        <v-row class="mt-5" justify="center">
          <v-col cols="10" lg="7" sm="6">
            <h1>Analytics</h1>
          </v-col>

          <v-col cols="4" lg="3" class="hidden-sm-and-down mt-2">
            <v-btn-toggle
              v-model="togglebtn"
              tile
              color="#DD1F25"
              group
            >
              <v-btn> Days </v-btn>

              <v-btn > Weeks </v-btn>

              <v-btn> Months </v-btn>
            </v-btn-toggle>
          </v-col>

          <v-col cols="4" lg="2" class="mt-2">
            <v-menu
              v-model="menu2"
              :close-on-content-click="false"
              :nudge-right="-115"
              transition="scale-transition"
              offset-y
              min-width="auto"
            >
              <template v-slot:activator="{ on, attrs }">
                <v-text-field
                  color="none"
                  solo
                  dense
                  v-model="date"
                  label="Select date"
                  prepend-icon="mdi-calendar"
                  readonly
                  v-bind="attrs"
                  v-on="on"
                ></v-text-field>
              </template>
              <v-date-picker
                v-model="date"
                @input="menu2 = false"
              ></v-date-picker>
            </v-menu>
          </v-col>
        </v-row>

        <v-row  justify="center">
          <div v-for="item in items" :key="item.title" class="px-3">
            <v-card width="275" height="140" class="pa-5" link>
              <v-list three-line>
                <v-list-item>
                  <v-list-item-content>
                    <v-list-item-subtitle class="font-weight-bold"
                      >{{ item.subtitle }}
                    </v-list-item-subtitle>

                    <v-list-item-title class="font-weight-bold">
                      {{ item.title }}
                    </v-list-item-title>

                    <v-list-item-subtitle class="font-weight-bold">
                      <span>{{ item.span }} </span>
                      {{ item.subtitle1 }}
                    </v-list-item-subtitle>
                  </v-list-item-content>
                  <v-list-item-action>
                    <v-btn icon v-model="icon" color="#DD1F25">
                      <v-icon>{{ item.icon }}</v-icon>
                    </v-btn>
                  </v-list-item-action>
                </v-list-item>
              </v-list>
            </v-card>
          </div>
        </v-row>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  data() {
    return {
      date: new Date(Date.now() - new Date().getTimezoneOffset() * 60000)
        .toISOString()
        .substr(0, 10),
      menu2: false,
      items: [
        {
          subtitle: "Total Sessions",
          title: "14K",
          span: "2.3%",
          subtitle1: "than last year",
          icon: "mdi-rotate-3d-variant",
        },
        {
          subtitle: "Total Bonus Rate",
          title: "56%",
          span: "2.1% ",
          subtitle1: "than last year",
          icon: "mdi-percent-outline",
        },
        {
          subtitle: "Total Revenues",
          title: "$768,342",
          span: "1.8%",
          subtitle1: "than last year",
          icon: "mdi-bitcoin",
        },
        {
          subtitle: "Total Users",
          title: "20K",
          span: "1.3%",
          subtitle1: "than last year",
          icon: "mdi-account-multiple-outline",
        },
      ],
      icon: [],
      togglebtn: 1,
    };
  },
};
</script>
