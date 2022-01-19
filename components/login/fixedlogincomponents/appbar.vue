<template>
  <div>
    <v-app-bar light flat text-lg-h2 text-md-h3 text-sm-h4>
      <p class="mt-3 ml-5 logo text-lg-h4 text-md-h5 text-sm-h6">
        LOGO
      </p>

      <v-spacer></v-spacer>
      <div class="hidden-sm-and-down">
        <v-btn text>
          <span>Home</span>
        </v-btn>

        <v-btn text>
          <span>About Us</span>
        </v-btn>

        <v-btn text>
          <span>Blogs</span>
        </v-btn>

        <v-btn text>
          <span>Contact Us</span>
        </v-btn>
      </div>

      <v-btn text class="btnlog" @click="loginDialog = true">
        <p class="login mt-4">
          <v-icon small class="mr-2">mdi-account-outline</v-icon>
          LOGIN
        </p>
      </v-btn>

      <v-divider vertical class="red mx-5"></v-divider>

      <v-btn depressed color="red" dark @click="signupDialog = true">
        Sign Up
      </v-btn>

      <div class="hidden-md-and-up">
        <v-app-bar-nav-icon @click="navicon = true"> </v-app-bar-nav-icon>
      </div>
    </v-app-bar>
    <v-spacer></v-spacer>
    <v-navigation-drawer
      right
      width="150"
      v-model="navicon"
      class="hidden-md-and-up mt-16"
      app
    >
      <v-list>
        <v-list-item>
          <v-list-item-content>
            <v-btn text>
              <span>Home</span>
            </v-btn>
          </v-list-item-content>
        </v-list-item>

        <v-list-item>
          <v-list-item-content>
            <v-btn text>
              <span>About Us</span>
            </v-btn>
          </v-list-item-content>
        </v-list-item>

        <v-list-item>
          <v-list-item-content>
            <v-btn text>
              <span>Blogs</span>
            </v-btn>
          </v-list-item-content>
        </v-list-item>

        <v-list-item>
          <v-list-item-content>
            <v-btn text>
              <span>Contact Us</span>
            </v-btn>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>

    <v-dialog v-model="loginDialog" max-width="450" ma>
      <v-card class="logshadow pl-5 pt-10 pr-10 pb-10">
        <h1 class="font-weight-bold text-center mb-3">Log in</h1>

        <v-col>
          <v-row>
            <v-col cols="3">
              <v-subheader class="mt-n4"> Email: </v-subheader>
            </v-col>
            <v-text-field
              dense
              solo
              autofocus
              required
              placeholder="Email"
              type="text"
              label="Email"
            ></v-text-field>
          </v-row>

          <v-row>
            <v-col cols="3">
              <v-subheader class="mt-n10"> Password: </v-subheader>
            </v-col>
            <v-text-field
              dense
              solo
              required
              placeholder="Password"
              type="Password"
              label="Password"
              class="mt-n5"
            >
            </v-text-field>
          </v-row>

          <v-row>
            <v-col align="center">
              <v-checkbox class="link mt-n1" label="Remember me"
                >Remember Me</v-checkbox
              >
            </v-col>
            <v-col align="center">
              <a href="#" class="link">Forgot Password? </a>
            </v-col>
          </v-row>

          <v-row class="ml-16">
            <v-btn type="sumbit" class="ml-16" color="red" dark>Log in</v-btn>
          </v-row>
        </v-col>
      </v-card>
    </v-dialog>

    <v-dialog v-model="signupDialog" max-width="870">
      <v-card>
        <v-row>
          <v-col cols="12" lg="5" class="red hidden-sm-and-down" align="center">
            <h1 class="pa-16">
              I Want to <br />
              become <br />
              A Donar
            </h1>
          </v-col>

          <v-col cols="12" lg="7">
            <v-card class="ma-10 pb-5" max-width="400">
              <h1 class="pt-10 mb-10 text-center">
                Donor Registration
              </h1>
              <v-row class="mt-n5">
                <v-col cols="3"><v-subheader>Name:</v-subheader></v-col>
                <v-col cols="8"
                  ><v-text-field
                    autofocus
                    dense
                    solo
                    type="text"
                    placeholder="Name"
                  >
                  </v-text-field
                ></v-col>
              </v-row>

              <v-row class="mt-n10">
                <v-col cols="3"> <v-subheader>Email:</v-subheader></v-col>
                <v-col cols="8"
                  ><v-text-field
                    label="Email"
                    dense
                    solo
                    type="email"
                    placeholder="Email"
                  >
                  </v-text-field
                ></v-col>
              </v-row>

              <v-row class="mt-n10">
                <v-col cols="3"><v-subheader> Number:</v-subheader></v-col>
                <v-col cols="8"
                  ><v-text-field
                    label=" Number"
                    dense
                    solo
                    type="number"
                    placeholder=" Number"
                  >
                  </v-text-field
                ></v-col>
              </v-row>

              <v-radio-group v-model="gender">
                <v-row class="mt-n15">
                  <v-col cols="3"><v-subheader>Gender:</v-subheader></v-col>
                  <v-radio
                    label="Male"
                    value="Male"
                    placeholder="Male"
                    class="mt-2 ml-5"
                  ></v-radio>
                  <v-radio
                    label="Female"
                    value="Female"
                    placeholder="Female"
                  ></v-radio>
                </v-row>
              </v-radio-group>

              <v-row class="mt-n10">
                <v-col cols="3"><v-subheader>Age:</v-subheader></v-col>
                <v-col cols="8"
                  ><v-text-field
                    label="Age"
                    dense
                    solo
                    type="number"
                    placeholder="Age"
                  >
                  </v-text-field
                ></v-col>
              </v-row>

              <v-row class="mt-n10">
                <v-col cols="3"> <v-subheader>Blood Group:</v-subheader></v-col>
                <v-col cols="8"
                  ><v-select
                    label="Select"
                    dense
                    solo
                    :items="select1"
                  ></v-select
                ></v-col>
              </v-row>

              <v-row class="mt-n10">
                <v-col cols="3"><v-subheader>Country:</v-subheader></v-col>
                <v-col cols="8"
                  ><v-select
                    label="Select"
                    dense
                    solo
                    :items="select2"
                  ></v-select
                ></v-col>
              </v-row>

              <v-row class="mt-n5 mb-5" justify="center">
                <v-btn
                  label="Registered"
                  type="submit"
                  placeholder="Registered"
                  color="red"
                  dark
                >
                  Registered
                </v-btn>
              </v-row>
            </v-card>
          </v-col>
        </v-row>
      </v-card>
    </v-dialog>
  </div>
</template>

<script>
export default {
  data() {
    return {
      gender: "",
      loginDialog: false,
      signupDialog: false,
      navicon: false,
      select1: [
        { text: "A" },
        { text: "B" },
        { text: "O" },
        { text: "AB" },
        { text: "-AB" },
        { text: "-A" },
        { text: "-B" },
        { text: "-O" },
      ],
      select2: [
        { text: "Nepal" },
        { text: "India" },
        { text: "China" },
        { text: "USA" },
        { text: "UAE" },
        { text: "UK" },
        { text: "Auatrila" },
        { text: "Korea" },
      ],
    };
  },
};
</script>

<style>
.login {
  color: #c71c1e;
}
.link {
  text-decoration: none;
  color: black !important;
  font-weight: bold;
}
.logshadow {
  box-shadow: 1px 1px 5px 1px rgba(0, 0, 0, 0.39) !important;
}
.logo {
  color: #c71c1e;
}
</style>
