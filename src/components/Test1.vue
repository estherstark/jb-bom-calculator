/* eslint-disable */
<template>
  <div>
    <v-toolbar color="grey darken-4" elevate-on-scroll>
      <a href="#default" class="logo">
        <img
          src="https://www.jenstore.com/media/wysiwyg/home/jbj-logo-footer.png"
          alt="JB Logo"
          style="height:30px;
          "
        />
      </a>
      <v-spacer />
      <v-toolbar-title class="white--text">JB BoM Calculator</v-toolbar-title>
      <v-spacer />
      <v-btn class="black--text" depressed color="yellow" accent-4>login</v-btn>
    </v-toolbar>
    <v-card class="pa-5 mx-lg-auto" outlined tile>
      <h2 class="font-weight-regular">Welcome to <br /></h2>
      <h1>JB BoM Calculator</h1>
      <img
        src="../assets/img-login.png"
        responsive
        style="max-width: 50%;
          max-height: 50%;"
      />
    </v-card>

    <v-container>
      <v-card class="pa-3 rounded-lg" color="grey lighten-3" width="400px">
        <h2 class="text-center">Please Log In</h2>

        <v-text-field
          label="Employee ID"
          color="white"
          outlined
          :rules="rules"
        ></v-text-field>
        <v-text-field
          label="Password"
          color="white"
          outlined
          :rules="rules"
        ></v-text-field>
        <v-btn class="login-btn" depressed color="yellow" accent-4>
          login
        </v-btn>
      </v-card>
    </v-container>
  </div>
</template>

<script>
export default {
  name: "Test1",
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
