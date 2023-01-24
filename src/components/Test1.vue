/* eslint-disable */
<template>
  <div>
    <v-toolbar color="grey darken-4" dense dark>
      <a href="#default" class="logo">
        <img
          src="https://www.jenstore.com/media/wysiwyg/home/jbj-logo-footer.png"
          alt="JB Logo"
          style="height:30px;"
        />
      </a>
      <v-spacer></v-spacer>
      <v-toolbar-title class="white--text">JB BoM Calculator</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn class="black--text" depressed color="yellow" accent-4>login</v-btn>
    </v-toolbar>

    <v-container
      v-for="align in alignments"
      :key="align"
      class="grey lighten-5 mb-6"
      ><v-row :align="align" no-gutters>
        <v-col>
          <v-card class="pa-8" outlined tile>
            <h2>Welcome to <br /></h2>
            <h1>JB BoM Calculator</h1>
            <img src="../assets/img-login.png" style="height:400px;" />
          </v-card>
        </v-col>
      </v-row>
    </v-container>

    <v-container fluid>
      <v-form>
        <v-text-field solo label="Append"></v-text-field>

        <v-card
          class="pa-md-4 mx-lg-auto"
          color="grey lighten-2"
          width="500px"
          elevation="1"
          text-center
          secondary
          text-no-wrap
          rounded-lg
        >
          <h2 class="text-subtitle-2 text-center">Please Log In</h2>

          <v-text-field
            label="Employee ID"
            outlined
            :rules="rules"
          ></v-text-field>
          <v-text-field label="Password" outlined :rules="rules"></v-text-field>
          <v-btn class="login-btn" depressed color="yellow" accent-4>
            login
          </v-btn>
        </v-card>
      </v-form>
    </v-container>
  </div>
</template>

<script>
export default {
  name: "Test1",
  data: () => ({
    alignments: ["start"]
  })
};
</script>

<style scoped>
.some-height {
  height: 100px;
  width: 100%;
}
</style>
