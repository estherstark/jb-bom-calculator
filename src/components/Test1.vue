/* eslint-disable */
<template>
  <div>
    <v-toolbar color="grey darken-4" dense dark>
      <v-toolbar-title>JB BoM Calculator</v-toolbar-title>
    </v-toolbar>

    <v-container>
      <v-row>
        <v-col></v-col>
      </v-row>
    </v-container>

    <h1>Welcome to <br />JB BoM Calculator</h1>
    <img src="../assets/img-login.png" max-height="10px" contain />
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
    alignments: ["start", "center", "end"]
  })
};
</script>

<style scoped>
.some-height {
  height: 100px;
  width: 100%;
}
</style>
