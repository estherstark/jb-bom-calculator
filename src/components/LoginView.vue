/* eslint-disable */
<template>
  <div>
    <v-app-bar>
      <v-toolbar color="grey darken-4" elevate-on-scroll>
        <a href="#default" class="logo">
          <img
            src="../assets/jb-logo-mini.png"
            alt="JB Logo"
            style="height:34px;"
            class="pa1"
          />
        </a>
        <v-spacer />
        <v-toolbar-title class="white--text hidden-sm-and-down"
          >JB BoM Calculator</v-toolbar-title
        >
        <v-spacer />
        <v-btn class="black--text" depressed color="yellow" accent-4>
          please login</v-btn
        >
      </v-toolbar>
    </v-app-bar>

    <v-container
      class="d-flex align-content-center flex-wrap"
      grid-list-lg
      responsive
    >
      <v-row justify="center" class="flex-wrap">
        <v-card class="pa-4 ma-2 d-flex justify-center align-center">
          <v-col class="order-2" style="min-width: 150px;" cols="12" md="1">
            <h2 class="font-weight-regular">Welcome to<br /></h2>
            <h1>JB BoM Calculator</h1>
            <img
              class="pb-3"
              src="../assets/img-login.png"
              responsive
              style="
            max-width: 80%;
            max-height: 80%;"
            />
          </v-col>

          <v-col class="order-1 pa-3 mr-4" cols="12" md="1">
            <v-card
              class="pa-4"
              color="grey lighten-3"
              style="min-width: 300px;
                     max-height: 300px;"
            >
              <v-layout column align-center>
                <h2>Please Log In</h2>
                <v-text-field label="Employee ID" outlined></v-text-field>
                <v-text-field label="Password" outlined></v-text-field>
                <v-btn class="login-btn" color="yellow" style="width: 50px">
                  login
                </v-btn>
              </v-layout>
            </v-card>
          </v-col>
        </v-card>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  name: "LoginView",
  data: () => ({
    alignments: ["start,end"]
  })
};
</script>

<style scoped>
.some-height {
  height: 100px;
  width: 100%;
}
</style>
