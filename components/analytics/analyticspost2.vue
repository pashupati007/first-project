<template>
  <div>
    <v-card class="pa-10 ma-10">
      <h1>Analytics traffic Channels & Goal</h1>
      <v-data-table
        mobile-breakpoint
        :headers="headers"
        :items="desserts"
        item-key="name"
        class="elevation-1 mt-5"
      >
      </v-data-table>

       <v-footer class="mt-5" color="white">
        <div class="text-center">
          <v-pagination
            v-model="page"
            :length="12"
            :total-visible="7"
            color="#DD1F25"
          ></v-pagination>
        </div>
      </v-footer>

    </v-card>
  </div>
</template>

<script>
export default {
  data: () => ({
    page: 1,
    headers: [
      {
        text: "CHANNELS",
        align: "start",
        sortable: false,
        value: "name",
      },
      { text: "SESSIONS", value: "sessions" },
      { text: "BONUS RATE", value: "bonucerate" },
      { text: "TRAFFIC", value: "traffic" },
      { text: "SALES", value: "sales" },
    ],
    desserts: [
      {
        name: "Direct",
        sessions: 67892,
        bonucerate: "26.3%",
        traffic: "8.1%",
        sales: 1132,
      },
      {
        name: "Call In",
        sessions: 89298,
        bonucerate: "42.2%",
        traffic: "1.5%",
        sales: 1856,
      },
      {
        name: "Paid Search",
        sessions: 62767,
        bonucerate: "9.3%",
        traffic: "6.0%",
        sales: 1449,
      },
      {
        name: "Organic Search",
        sessions: 123879,
        bonucerate: "45.9%",
        traffic: "7.5%",
        sales: 1432,
      },
      {
        name: "Email",
        sessions: 92179,
        bonucerate: "48.2%",
        traffic: "4.2%",
        sales: 2029,
      },
      {
        name: "Referal",
        sessions: 15875,
        bonucerate: "31.1%",
        traffic: "3.2%",
        sales: 1689,
      },
      {
        name: "Proposal",
        sessions: 92179,
        bonucerate: "48.2%",
        traffic: "4.2%",
        sales: 2029,
      },
    ],
  }),
};
</script>

<style>
.v-data-footer {
  display: none;
}
</style>
