<template>
  <div>
    <v-row class="mt-10">
      <v-col cols="12" lg="9">
          <v-card class="mx-auto" max-width="850">
          <v-toolbar flat>
            <v-toolbar-title>New Customers</v-toolbar-title>
          </v-toolbar>

          <v-list subheader>
            <v-list-item v-for="chat in recent" :key="chat.title" link>
              <v-list-item-avatar>
                <v-img :alt="`${chat.title} avatar`" :src="chat.avatar"></v-img>
              </v-list-item-avatar>

              <v-list-item-content>
                <v-list-item-title v-text="chat.title"></v-list-item-title>
                <v-list-item-subtitle
                  v-text="chat.subtitle"
                ></v-list-item-subtitle>
              </v-list-item-content>

              <v-list-item-icon>
                <v-icon>
                  mdi-email-outline
                </v-icon>
              </v-list-item-icon>
            </v-list-item>
          </v-list>
        </v-card>
      </v-col>

      <v-col cols="12" lg="3">
        <v-card class="mx-auto" max-width="290">
          <v-toolbar flat>
            <v-toolbar-title>New Customers</v-toolbar-title>
          </v-toolbar>

          <v-list subheader>
            <v-list-item v-for="chat in recent" :key="chat.title" link>
              <v-list-item-avatar>
                <v-img :alt="`${chat.title} avatar`" :src="chat.avatar"></v-img>
              </v-list-item-avatar>

              <v-list-item-content>
                <v-list-item-title v-text="chat.title"></v-list-item-title>
                <v-list-item-subtitle
                  v-text="chat.subtitle"
                ></v-list-item-subtitle>
              </v-list-item-content>

              <v-list-item-icon>
                <v-btn icon>
                  <v-icon v-text="chat.icon">
                </v-icon>
                </v-btn>
              </v-list-item-icon>
            </v-list-item>
          </v-list>

          <v-divider inset></v-divider>

          
              <v-menu label="More In Sights">More In Sights</v-menu>
        <v-expansion-panels>
    <v-expansion-panel>
      <v-expansion-panel-header>
        More In Sights
      </v-expansion-panel-header>
      <v-expansion-panel-content>
      </v-expansion-panel-content>
    </v-expansion-panel>
  </v-expansion-panels>
        </v-card>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  data: () => ({
    recent: [
      {
        active: true,
        avatar: "https://cdn.vuetifyjs.com/images/lists/1.jpg",
        title: "Mitchell Williamson",
        subtitle: "Customer ID#01220",
        icon: "mdi-email-outline",
      },
      {
        active: true,
        avatar: "https://cdn.vuetifyjs.com/images/lists/2.jpg",
        title: "Sam Conner",
        subtitle: "Customer ID#01221",
        icon: "mdi-email-outline",
      },
      {
        avatar: "https://cdn.vuetifyjs.com/images/lists/3.jpg",
        title: "Christian Castro",
        subtitle: "Customer ID#01222",
        icon: "mdi-email-outline",
      },
      {
        avatar: "https://cdn.vuetifyjs.com/images/lists/4.jpg",
        title: "Harriett Clark",
        subtitle: "Customer ID#01223",
        icon: "mdi-email-outline",
      },
    ],
  }),
};
</script>
