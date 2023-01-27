<template>
  <v-app-bar absolute elevate-on-scroll>
    <v-toolbar color="grey darken-4" elevate-on-scroll>
      <a href="https://www.jenbunjerd.com/" target="_blank">
        <img
          src="../assets/jb-logo-mini.png"
          alt="JB Logo"
          style="height:34px;"
          class="pa1"
        />
      </a>

      <v-app-bar-title class="pl-3 toolbar-title hidden-sm-and-down"
        >JB BoM Calculator</v-app-bar-title
      >
      <v-spacer />

      <router-link v-if="!isLoggedIn" to="/login">
        <v-btn class="btn" color="white" accent-4>
          Plese login</v-btn
        ></router-link
      >
      <span v-if="isLoggedIn">
        <v-btn class="btn" accent-4> Employee ID</v-btn></span
      >
      <router-link v-if="isLoggedIn" to="/logout">
        <v-btn class="btn" color="deep-orange accent-2" accent-4>
          Log Out</v-btn
        ></router-link
      >
    </v-toolbar>
  </v-app-bar>
</template>

<script>
export default {
  name: "Appbar",
  data() {
    return {
      isLoggedIn: false,
      username: ""
    };
  },
  methods: {
    login() {
      // Code to handle login
      this.isLoggedIn = true;
      this.username = "John Doe";
    },
    logout() {
      // Code to handle logout
      this.isLoggedIn = false;
      this.username = "";
    }
  }
};
</script>

<style>
.toolbar-title {
  font-family: Arial, Helvetica, sans-serif;
  font-size: 25px;
  font-weight: bold;
  color: white;
}
.btn {
  font-family: Arial, Helvetica, sans-serif;
  font-weight: normal;
  color: black;
  border-radius: 8px;
}
</style>
