<template>
  <div>
   <v-container>
      <v-navigation-drawer app clipped>
      <v-list dense>
        <v-list-item>
          <v-list-item-avatar>
            <img :src="require('~/assets/img/loginimg/blog2.png')" />
          </v-list-item-avatar>

          <v-list-item-content>
            <v-list-item-title>
              <h1 class="navtitle mt-5">Give Blood</h1>
            </v-list-item-title>

            <v-list-item-subtitle>
              <v-select solo :items="navdslt" label="Ready to donate">
                Ready to donate
              </v-select>
            </v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>
      </v-list>

      <v-list>
        <v-list-item v-for="(item, i) in items" :key="i" :to="item.link">
          <v-list-item-icon>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-icon>
          <v-list-item-content>
            <v-list-item-title>
              {{ item.title }}
            </v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>

        <div class="text-center mt-15">
           <v-btn color="#DD1F25" dark width="250" Elevation>
        <h3>Logout</h3>
      </v-btn>
      </div>

    </v-navigation-drawer>
   </v-container>
  </div>
</template>

<script>
export default {
  data() {
    return {
      navdslt: [{ text: " Ready to donate " }, { text: " Ready to donate " }],
      items: [
        { title: "Bloodfeeds",icon: 'mdi-emoticon',link: "/homepages/bloodfeeds" },
        { title: "Blood Banks",icon: 'mdi-emoticon', link: "/homepages/bloodbank" },
        { title: "Donars",icon: 'mdi-emoticon', link: "/homepages/donors" },
        { title: "Blood records",icon: 'mdi-emoticon', link: "/homepages/bloodrecords" },
        { title: "Blogs",icon: 'mdi-emoticon', link: "/homepages/blogs" },
        { title: "Setting",icon: 'mdi-emoticon', link: "/homepages/setting" },
      ],
    };
  },
};
</script>

<style>
.navtitle {
  color: #dd1f25;
}
</style>
