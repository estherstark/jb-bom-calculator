<template>
  <v-app>
    <div id="app">
      <InputSetView />
    </div>
  </v-app>
</template>

<script>
// eslint-disable-next-line
import LoginView from "./components/LoginView";
import InputJobView from "./components/InputJobView";
import SvgIcon from "@jamescoyle/vue-icon";
import InputSetView from "./components/InputSetView";

export default {
  name: "App",
  components: {
    LoginView,
    InputJobView,
    InputSetView
  }
};
</script>

<style></style>
