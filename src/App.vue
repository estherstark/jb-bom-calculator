<template>
  <v-app>
    <div id="app">
      <LoginView />
    </div>
  </v-app>
</template>

<script>
// eslint-disable-next-line
import LoginView from "./components/LoginView.vue";

export default {
  name: "App",
  components: {
    LoginView
  }
};
</script>

<style></style>
