<template>
  <div>
    <container>
      <v-navigation-drawer permanent>
        <v-card>
          <v-list dense>
            <v-list-item>
              <v-list-item-avatar>
                <img :src="require('~/assets/img/blog2.png')" alt="" />
              </v-list-item-avatar>

              <v-list-item-content>
                <v-list-item-title>
                  <h1 class="navtitle">
                    Give Blood
                  </h1>
                </v-list-item-title>
                <v-list-item-subtitle>
                  <v-select solo :items="navdslt">
                    Ready to donate
                  </v-select>
                </v-list-item-subtitle>
              </v-list-item-content>
            </v-list-item>
          </v-list>

          <v-list class="ml-16">
              <v-list-item>
                <v-list-item-content>
                  <v-list-item-title>
                    Bloodfeeds
                  </v-list-item-title>
                </v-list-item-content>
              </v-list-item>

              <v-list-item>
                <v-list-item-content>
                  <v-list-item-title>
                    Blood Banks
                  </v-list-item-title>
                </v-list-item-content>
              </v-list-item>

            <v-list-item>
              <v-list-item-content>
                <v-list-item-title>
                  Donars
                </v-list-item-title>
              </v-list-item-content>
            </v-list-item>

            <v-list-item>
              <v-list-item-content>
                <v-list-item-title>
                  Blood records
                </v-list-item-title>
              </v-list-item-content>
            </v-list-item>

            <v-list-item>
              <v-list-item-content>
                <v-list-item-title>
                  Blogs
                </v-list-item-title>
              </v-list-item-content>
            </v-list-item>

            <v-list-item>
              <v-list-item-content>
                <v-list-item-title>
                  Setting
                </v-list-item-title>
              </v-list-item-content>
            </v-list-item>
          </v-list>

          <v-footer class="red">
            <p class="navfooter ml-16">
              <v-icon dark>mdi-logout</v-icon>
              Logout
            </p>
          </v-footer>
        </v-card>
      </v-navigation-drawer>
    </container>
  </div>
</template>

<script>
export default {
  data() {
    return {
      
      navdslt : [
        { text: " Ready to donate " },
        { text: " Ready to donate " },
      ],

    };
  },
};
</script>


<style>
.navtitle {
  color: red;
}
.navfooter{
  color: white;
}
</style>
