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
    alignments: ["start,end"]
  })
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
</style>
