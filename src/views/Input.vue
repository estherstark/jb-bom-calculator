<template>
  <v-app background-color="white">
    <h1 class="ma-4 font-weight-regular">
      Input Details for Calculating
    </h1>

    <v-card>
      <v-tabs
        vertical
        v-model="active"
        color="black"
        dark
        slider-color="yellow"
      >
        <v-tab v-for="n in 3" :key="n" ripple> Set {{ n }} </v-tab>
        <v-tab-item v-for="n in 3" :key="n">
          <v-card flat>
            <v-card-text> </v-card-text>
          </v-card>
        </v-tab-item>
      </v-tabs>
    </v-card>
  </v-app>
</template>

<script>
export default {
  name: "InputCal",
  data: () => ({
    rackType: ["Selective Rack", "Long Span Rack", "Micro Rack"],
    text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit."
  }),

  /* eslint-env browser */
  methods: {
    next() {
      const active = parseInt(this.active, 10);
      this.active = active < 2 ? active + 1 : 0;
    },
    cal() {}
  }
};
</script>

<style scoped>
.some-height {
  height: 100px;
  width: 100%;
}
.v-btn--outlined {
  border: thin solid #ffd600;
}
.text-input {
  border-radius: 8px;
}
</style>
