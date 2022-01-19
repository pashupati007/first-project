<template>
  <div>
    <v-container>
      <v-data-table :headers="headers" :items="blood_bank" class="elevation-1">
        <template v-slot:top>
          <v-toolbar flat>
            <v-toolbar-title>Outside Valley</v-toolbar-title>
          </v-toolbar>
        </template>
      </v-data-table>

      <v-footer class="mt-5">
        <div class="text-center">
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
          blood_bank_center: "Dhulikhel Hospital",
          address: "Dhulikhel",
          contact_number: "9815779141",
        },
        {
          blood_bank_center: "Dharan Blood Transfusion Service",
          address: "Dharan",
          contact_number: "9815779141",
        },
        {
          blood_bank_center: "Dhanusa Blood Transfusion Service",
          address: "Dhanusa",
          contact_number: "9815779141",
        },
        {
          blood_bank_center: "Bharatpur Blood Transfusion Service",
          address: "Bharatpur",
          contact_number: "9815779141",
        },
        {
          blood_bank_center: "Jhapa Blood Transfusion Service",
          address: "Jhapa",
          contact_number: "9815779141",
        },
        {
          blood_bank_center: "Pokhara Blood Transfusion Service",
          address: "Pokhara",
          contact_number: "9815779141",
        },
      ],
    };
  },
};
</script>
