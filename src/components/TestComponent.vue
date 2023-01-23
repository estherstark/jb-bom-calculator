<template>
  <div>
    <v-toolbar dark color="grey darken-3">
      <v-toolbar-side-icon>
        <v-img src="https://www.jenbunjerd.com/images/logo-menu.png" />
      </v-toolbar-side-icon>
      <v-toolbar-title>JB BoM Calculator</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn icon>
        <v-icon>search</v-icon>
      </v-btn>
      <v-btn icon>
        <v-icon>refresh</v-icon>
      </v-btn>
      <v-btn icon>
        <v-icon>more_vert</v-icon>
      </v-btn>
    </v-toolbar>

    <div>
      <v-tabs v-model="active" color="cyan" dark slider-color="yellow">
        <v-tab v-for="n in 3" :key="n" ripple> Set {{ n }} </v-tab>
        <v-tab-item v-for="n in 3" :key="n">
          <v-card flat>
            <v-card-text>{{ text }}</v-card-text>
          </v-card>
        </v-tab-item>
      </v-tabs>
    </div>

    <v-layout>
      <v-flex xs12 sm6 offset-sm3>
        <v-card>
          <v-card-media
            src="https://cdn.vuetifyjs.com/images/cards/desert.jpg"
            height="200px"
          ></v-card-media>

          <v-card-title primary-title>
            <div>
              <h3 class="headline mb-0">Kangaroo Safari</h3>
              <div>
                Located two hours south of Sydney in the <br />Southern
                Highlands of New South Wales, ...
              </div>
            </div>
          </v-card-title>

          <v-card-actions>
            <v-btn flat color="orange">Share</v-btn>
            <v-btn flat color="orange">Explore</v-btn>
          </v-card-actions>
        </v-card>
      </v-flex>
    </v-layout>
    <div class="text-xs-center mt-3">
      <v-btn color="white" v-on:click="next">next</v-btn>
    </div>
  </div>
</template>

<script>
import SplitPane from "vue-splitpane";

export default {
  name: "TestComponent",
  data() {
    return {
      msg: "Message goes here",
      items: [{ title: "one" }, { title: "two" }],
      active: null,
      text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit."
    };
  },
  /* eslint-env browser */
  methods: {
    next() {
      const active = parseInt(this.active, 10);
      this.active = active < 2 ? active + 1 : 0;
    },

    resize() {
      // eslint-disable-next-line no-console
      // eslint-disable-next-line
      console.log("resized");
    }
  },
  components: {
    SplitPane
  }
};
</script>

<style scoped>
.some-height {
  height: 100px;
  width: 100%;
}
</style>
