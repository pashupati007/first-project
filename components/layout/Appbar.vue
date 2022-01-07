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

        <v-btn text class="btnlog" @click="loginDialog = true">
          <p class="login mt-4">
            <v-icon small class="mr-2">mdi-account-outline</v-icon>
            LOGIN
          </p>
        </v-btn>
      </div>
      <v-divider vertical class="red mx-5"></v-divider>

      <v-btn depressed color="red" dark @click="signupDialog = true">
        Sign Up
      </v-btn>
    </v-app-bar>

    <div class="hidden-md-and-up">
menu
    </div>

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

    <v-dialog v-model="signupDialog" max-width="700">
      <v-card>
        <v-row>
          <v-col cols="5" align="center">
            <p>
              I Want to <br />
              become <br />
              A Donar
            </p>
          </v-col>

          <v-col cols="7">
            <v-card class="pa-10">
              <h1 class="mt-5 mb-5 text-center">
                Donor Registration
              </h1>
              <v-row>
                <v-subheader>Name:</v-subheader>
                <v-text-field autofocus dense solo type="text"  placeholder="Name"> </v-text-field>
              </v-row>
                <v-col cols="3"><v-subheader>Email:</v-subheader></v-col>
                <v-text-field dense solo type="email" class="mt-n7"  placeholder="Email">
                </v-text-field>

                <v-col cols="3"><v-subheader>Phone Number:</v-subheader></v-col>
                <v-text-field dense solo type="number" class="mt-n14"  placeholder="Phone Number">
                </v-text-field>

                <v-col cols="12" class="mt-n16">
                  <v-row>
                    <v-subheader>Gender:</v-subheader>
                    <v-radio label="Male" value="Male" placeholder="Male"></v-radio>
                    <v-radio label="Female" value="Female" placeholder="Female"></v-radio>
                  </v-row>
                </v-col>

                <v-col cols="3"><v-subheader>Age:</v-subheader></v-col>
                <v-text-field dense solo type="number"  placeholder="Age"> </v-text-field>

                <v-col cols="12">
                  <v-row>
                    <v-subheader>Blood Group:</v-subheader>
                    <v-select label="Select" solo></v-select>
                  </v-row>
                </v-col>

                <v-col cols="12">
                  <v-row>
                    <v-subheader>Country:</v-subheader>
                    <v-select label="Select" solo></v-select>
                  </v-row>
                </v-col>
                <v-row>
                <v-col cols="" align="center"
                  ><v-btn label="registered" type="submit"
                    >Registered</v-btn
                  ></v-col
                >
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
      loginDialog: false,
      signupDialog: false,
    };
  },
};
</script>

<style lang="css">
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
