<template>
  <div>
    <v-app-bar dense flat app clipped-left color="white">
      <v-toolbar-title>im.pek.a.ble</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-text-field
        solo
        dense
        label="Search"
        prepend-inner-icon="mdi-magnify"
        class="size mt-6"
        color="none"
        flat
      >
      </v-text-field>
      <v-spacer></v-spacer>
      <v-spacer></v-spacer>

      <v-btn icon>
        <v-icon>mdi-chat-processing-outline</v-icon>
      </v-btn>

      <v-btn icon>
        <v-icon>mdi-bell-outline</v-icon>
      </v-btn>

      <v-btn icon>
        <v-icon>mdi-google-maps</v-icon>
      </v-btn>

      <v-avatar><img :src="require('~/assets/img/loginimg/blog3.png')"></v-avatar>

      <v-menu class="mt-6" dense solo></v-menu>

      <v-menu offset-y>
        <template v-slot:activator="{ on, attrs }">
          <v-btn v-bind="attrs" v-on="on">
            Dropdown
          </v-btn>
        </template>
        <v-list>
          <v-list-item v-for="(item, index) in items" :key="index">
            <v-list-item-title>{{ item.title }}</v-list-item-title>
          </v-list-item>
        </v-list>
      </v-menu>
    </v-app-bar>
  </div>
</template>

<script>
export default {
  data: () => ({
    items: [
      { title: "Click Me" },
      { title: "Click Me" },
      { title: "Click Me" },
      { title: "Click Me 2" },
    ],
  }),
};
</script>

<style>
.size {
  width: 2px;
}
</style>
