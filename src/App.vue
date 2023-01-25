<template>
  <v-app>
    <div id="app">
      <InputJobView />
    </div>
  </v-app>
</template>

<script>
// eslint-disable-next-line
import LoginView from "./components/LoginView.vue";
import InputJobView from "./components/InputJobView.vue";
import SvgIcon from '@jamescoyle/vue-icon'


export default {
  name: "App",
  components: {
    LoginView,
    InputJobView
  }
};
</script>

<style></style>
