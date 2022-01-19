<template>
  <div>
    <v-container>
      <v-data-table
        :headers="headers"
        :items="country0"
        :search="search"
        sort-by="country"
        class="elevation-1"
      >
        <template v-slot:top>
          <v-toolbar flat>
            <v-toolbar-title>COUNTRY</v-toolbar-title>
            <v-divider class="mx-4" inset vertical></v-divider>
            <v-spacer></v-spacer>
            <v-text-field
              v-model="search"
              append-icon="mdi-magnify"
              label="Search"
              single-line
              hide-details
              color="#57B8FF"
            ></v-text-field>
            <v-spacer></v-spacer>
            <v-dialog v-model="dialog" max-width="400px">
              <template v-slot:activator="{ on, attrs }">
                <v-btn
                  color="#57B8FF"
                  dark
                  class="mb-2"
                  v-bind="attrs"
                  v-on="on"
                  v-model="valid"
                >
                  ADD COUNTRY
                </v-btn>
              </template>

              <v-card>
                <v-card-title>
                  <span class="text-h5">{{ formTitle }}</span>
                </v-card-title>

                <v-card-text>
                  <v-container>
                    <v-row>
                      <v-col>
                        <v-form v-model="valid" ref="form">
                          <v-text-field
                            v-model="editedItem.country"
                            label="country name"
                            :rules="countryRules"
                          ></v-text-field>
                        </v-form>
                      </v-col>
                    </v-row>
                  </v-container>
                </v-card-text>

                <v-card-actions>
                  <v-spacer></v-spacer>
                  <v-btn color="#57B8FF" text @click="close"> Cancel </v-btn>
                  <v-btn color="#57B8FF" text @click="save"> Save </v-btn>
                </v-card-actions>
              </v-card>
            </v-dialog>
            <v-dialog v-model="dialogDelete" max-width="400px">
              <v-card>
                <v-card-title class="text-h5"
                  >Are you sure you want to delete this item?</v-card-title
                >
                <v-card-actions>
                  <v-spacer></v-spacer>
                  <v-btn color="#57B8FF" text @click="closeDelete"
                    >Cancel</v-btn
                  >
                  <v-btn color="#57B8FF" text @click="deleteItemConfirm"
                    >OK</v-btn
                  >
                  <v-spacer></v-spacer>
                </v-card-actions>
              </v-card>
            </v-dialog>
          </v-toolbar>
        </template>
        <template v-slot:item.actions="{ item }">
          <v-icon small class="mr-2" @click="editItem(item)">
            mdi-pencil
          </v-icon>

          <v-icon small @click="deleteItem(item)"> mdi-delete </v-icon>
        </template>
        <template v-slot:no-data>
          <v-btn color="#57B8FF" @click="initialize"> Reset </v-btn>
        </template>
      </v-data-table>
    </v-container>
  </div>
</template>

<script>
export default {
  data: () => ({
    search: "",

    countryRules: [(v) => !!v || "Country is required"],
    dialog: false,
    dialogDelete: false,
    headers: [
      {
        text: "S.N.",
        align: "start",
        sortable: false,
        value: "name",
      },
      { text: "COUNTRY", value: "country", sortable: false },
      { text: "Actions", value: "actions", sortable: false },
    ],
    country0: [{}],
    editedIndex: -1,
    editedItem: {
      name: "",
      country: "",
    },
    defaultItem: {
      name: "",
      country: "",
    },
  }),

  computed: {
    formTitle() {
      return this.editedIndex === -1 ? "NEW COUNTRY" : "ADD COUNTRY";
    },
  },

  watch: {
    dialog(val) {
      val || this.close();
    },
    dialogDelete(val) {
      val || this.closeDelete();
    },
  },

  created() {
    this.initialize();
  },

  methods: {
    valid: true,
    initialize() {
      this.country0 = [
        {
          name: "1",
          country: "Nepal",
        },
      ];
    },

    editItem(item) {
      console.log(item);
      // this.editedIndex = this.country0.indexOf(item);
      // this.editedItem = Object.assign({}, item);
      // this.dialog = true;
    },

    deleteItem(item) {
      this.editedIndex = this.country0.indexOf(item);
      this.editedItem = Object.assign({}, item);
      this.dialogDelete = true;
    },

    deleteItemConfirm() {
      this.country0.splice(this.editedIndex, 1);
      this.closeDelete();
    },

    close() {
      this.dialog = false;
      this.$nextTick(() => {
        this.editedItem = Object.assign({}, this.defaultItem);
        this.editedIndex = -1;
      });
    },

    closeDelete() {
      this.dialogDelete = false;
      this.$nextTick(() => {
        this.editedItem = Object.assign({}, this.defaultItem);
        this.editedIndex = -1;
      });
    },

    save() {
      if (this.$refs.form.validate()) {
        if (this.editedIndex > -1) {
          Object.assign(this.country0[this.editedIndex], this.editedItem);
        } else {
          this.country0.push(this.editedItem);
        }
        this.close();
      }

    },
  },
};
</script>