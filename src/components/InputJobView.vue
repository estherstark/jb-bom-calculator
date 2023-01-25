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
          please login</v-btn
        >
      </v-toolbar>
    </v-app-bar>
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