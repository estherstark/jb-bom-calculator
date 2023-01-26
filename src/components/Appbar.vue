<template>
  <v-app-bar>
    <v-toolbar color="grey darken-4" elevate-on-scroll>
      <a href="https://www.jenbunjerd.com/" target="_blank">
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

      <router-link v-if="!isLoggedIn" to="/login">
        <v-btn class="black--text" depressed color="yellow" accent-4>
          Plese login</v-btn
        ></router-link
      >
      <span v-if="isLoggedIn">
        <v-btn class="black--text" depressed color="yellow" accent-4>
          Employee ID</v-btn
        ></span
      >
      <router-link v-if="isLoggedIn" to="/logout">
        <v-btn
          class="black--text"
          depressed
          color="deep-orange accent-2"
          accent-4
        >
          Log Out</v-btn
        ></router-link
      >
    </v-toolbar>
  </v-app-bar>

  <!--<template>
  <div>
    <nav>
      <router-link to="/">Home</router-link>
      <router-link to="/about">About</router-link>
      <router-link v-if="!isLoggedIn" to="/login">Login</router-link>
      <span v-if="isLoggedIn">{{username}}</span>
      <router-link v-if="isLoggedIn" to="/logout">Logout</router-link>
    </nav>
    <router-view/>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isLoggedIn: false,
      username: ""
    }
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
}
</script> -->
</template>

<script>
export default {
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
