<template>
  <div class="hello">
    <div id="appbar"><Appbar /></div>
    <div id="app">
      <Input />
    </div>
  </div>
</template>

<script>
// eslint-disable-next-line
import Appbar from "./components/Appbar";
import Login from "./views/Login";
import Input from "./views/Input";
import InputJobView from "./components/InputJobView";
import InputCal from "./components/InputCal";
import OutputPreview from "./components/OutputPreview";
import HelloWorldVue from "./components/HelloWorld";
import TestComponent from "./components/TestComponent";

export default {
  name: "App",
  components: {
    Appbar,
    Login,
    Input,
    InputJobView,
    InputCal,
    OutputPreview,
    HelloWorldVue,
    TestComponent
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 10px;
}
</style>
