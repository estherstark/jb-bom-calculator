<template>
  <v-app>
    <div id="app">
      <TestComponent/>
    </div>
  </v-app>
</template>

<script>
import HelloWorld from "./components/HelloWorld";
import TestComponent from './components/TestComponent.vue'

export default {
  name: "App",
  components: {
    HelloWorld,
    TestComponent,
  }
};
</script>

<style>
</style>
