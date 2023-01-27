<template>
  <v-app>
    <h1 class="ma-4 font-weight-regular">
      Input Details for Calculating
    </h1>
  </v-app>
</template>

<script>
export default {
  name: "InputCal",
  data: () => ({
    rackType: ["Selective Rack", "Long Span Rack", "Micro Rack"]
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
