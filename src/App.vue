<template>
  <v-app>
    <div id="app">
      <Appbar />
    </div>
  </v-app>
</template>

<script>
// eslint-disable-next-line
import LoginView from "./components/LoginView";
import InputJobView from "./components/InputJobView";
import InputSetView from "./components/InputSetView";
import Appbar from "./components/Appbar";
import HelloWorldVue from "./components/HelloWorld.vue";

export default {
  name: "App",
  components: {
    LoginView,
    InputJobView,
    InputSetView,
    Appbar,
    HelloWorldVue
  }
};
</script>

<style></style>
