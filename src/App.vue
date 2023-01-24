<template>
  <v-app>
    <div id="app">
      <Test1Vue />
    </div>

    <v-app-bar app>
      <!-- -->
    </v-app-bar>

    <!-- Sizes your content based upon application components -->
    <v-main>
      <!-- Provides the application the proper gutter -->
      <v-container fluid>
        <!-- If using vue-router -->
        <router-view></router-view>
      </v-container>
    </v-main>

  </v-app>
</template>

<script>
import HelloWorld from "./components/HelloWorld";
// eslint-disable-next-line
import TestComponent from "./components/TestComponent.vue";
// eslint-disable-next-line
import Test1Vue from "./components/Test1.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
    TestComponent,
    Test1Vue
  }
};
</script>

<style></style>
