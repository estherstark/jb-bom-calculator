<template>
  <v-app>
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
          Employee ID</v-btn
        >
      </v-toolbar>
    </v-app-bar>
    <h1 class="ma-4 font-weight-regular text-center">
      Input Job Details
    </h1>
    <v-card>
      <v-text-field
        label="Enter Job Name/ID"
        :rules="rules"
        hide-details="auto"
      ></v-text-field>
      <v-text-field
        label="Enter Number of Set"
        :rules="rules"
        hide-details="auto"
      ></v-text-field>

      <v-btn class="black--text" depressed color="yellow" border 1px solid white;'> Next ></v-btn>
    </v-card>
  </v-app>
</template>

<script>
export default {
  name: "ImportJobView",
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
