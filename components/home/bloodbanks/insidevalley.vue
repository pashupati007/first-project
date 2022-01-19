<template>
  <div>
    <v-container>
        <v-data-table :headers="headers" :items="blood_bank" class="elevation-1">
        <template v-slot:top>
          <v-toolbar flat>
            <v-toolbar-title>In Kathmandu Valley</v-toolbar-title>
          </v-toolbar>
        </template>
      </v-data-table>

      <v-footer class="mt-5">
        <div class="text-center" >
          <v-pagination
            v-model="page"
            :length="15"
            :total-visible="7"
            prev-icon="mdi-menu-left"
            next-icon="mdi-menu-right"
            color="#DD1F25"
          ></v-pagination>
        </div>
      </v-footer>
    </v-container>
  </div>
</template>

<script>
export default {
  data() {
    return {
      page: 1,
      headers: [
        { text: "Blood Bank Center", value: "blood_bank_center" },
        { text: "Address", value: "address" },
        { text: "Contact Number", value: "contact_number" },
      ],
      blood_bank: [
        {
          blood_bank_center: "Bir Hospital",
          address: "New Road Gate,Kathmandu",
          contact_number: "01-6623541",
        },
        {
          blood_bank_center: "Central Blood Transfusion Center",
          address: "Soltimode,Kalimati",
          contact_number: "01-6623541",
        },
        {
          blood_bank_center: "Red Cross Society",
          address: "Lalitpur",
          contact_number: "01-6623541",
        },
        {
          blood_bank_center: "Grande International Hospital",
          address: "Tokha,Kathmandu",
          contact_number: "01-6623541",
        },
        {
          blood_bank_center: "",
          address: "Maharajgunj,Kathmandu",
          contact_number: "01-6623541",
        },
        {
          blood_bank_center: "Bhaktapur Hospital",
          address: "Bhaktapur",
          contact_number: "01-6623541",
        },
      ],
    };
  },
};
</script>
