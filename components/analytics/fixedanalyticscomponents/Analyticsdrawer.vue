<template>
  <div>
    <v-navigation-drawer app clipped>
      <v-list nav click>
            <div v-for="(item,i) in items" :key="i">
                <v-list-group v-if="item.subGroup" color="none">
                    <template v-slot:activator>
                        <v-list-item-icon>
                            <v-icon>{{item.icon}}</v-icon>
                        </v-list-item-icon>
                        <v-list-item-content>
                            <v-list-item-title>{{item.title}}</v-list-item-title>
                        </v-list-item-content>
                    </template>
                    <div>
                        <v-list-item v-for="(sub,j) in item.subGroupItem" :key="j" :to="sub.link" class="pl-13">
                            <v-list-item-icon>
                        <v-icon>{{sub.icon}}</v-icon>
                    </v-list-item-icon>
                    <v-list-item-content>
                        <v-list-item-title>{{sub.title}}</v-list-item-title>
                    </v-list-item-content>
                        </v-list-item>
                    </div>
                </v-list-group>
                <v-list-item v-else :to="item.link">
                    <v-list-item-icon>
                        <v-icon>{{item.icon}}</v-icon>
                    </v-list-item-icon>
                    <v-list-item-content>
                        <v-list-item-title>{{item.title}}</v-list-item-title>
                    </v-list-item-content>
                </v-list-item>
            </div>
        </v-list>

    </v-navigation-drawer>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        { title: "Home", 
          icon: "mdi-home-outline",
          subGroup: false,
          link: '/home',
        },
        { title: "Analytics", 
          icon: "mdi-google-analytics",
          subGroup: false,
          link: '/adminpages/analytics',
        },
        { title: "User",
          icon: "mdi-account-circle-outline",
          subGroup: false, 
          link: '/adminpages/user',
        },
        { title: "Location",
          icon: "mdi-google-maps",
          subGroup: true,
          subGroupItem: [
                        {
                          title: 'Country',
                          icon: "mdi-google-maps",
                          link: '/adminpages/country',
                        },
                        {
                          title: 'City',
                          icon: "mdi-city",
                          link: '/adminpages/city',
                        },
                        {
                          title: 'State',
                          icon: "mdi-google-maps",
                          link: '/adminpages/state',
                        },
                        ],          
        },
        { title: "Post",
          icon: "mdi-post-outline",
          subGroup: false,
          link: '/adminpages/post',
        },
        { title: "Blog",
          icon: "mdi-notebook-outline",
          subGroup: false,
          link: '/adminpages/blog',
        },
        { title: "Blood Bank",
          icon: "mdi-blood-bag",
          subGroup: false,
          link: '/adminpages/blood_bank',
        },
        { title: "Donor Request",
          icon: "mdi-calendar-minus",
          subGroup: false,
          link: '/adminpages/donor_request',
        },
      ],
      model: 1,
    };
  },
};
</script>