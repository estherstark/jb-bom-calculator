<template>
  <v-app>
    <h1 class="ma-4 font-weight-regular">
      Input Details for Calculating
    </h1>

    <v-card
      class="pa-4 ma-2 d-flex justify-center align-center"
      color="grey lighten-3"
      style="min-width: 300px;"
    >
      <v-layout column align-center class="mt-3 mb-3" v-for="n in 2" :key="n">
        <v-row>
          <v-col>
            <span>Set {{ n }}: </span>
            <v-text-field
              outlined
              placeholder="Enter Set Name/ID"
              type="text"
              max-width="200px"
            ></v-text-field>

            <span>Number of Set:</span>

            <v-text-field
              outlined
              placeholder="Enter Number of Set"
              type="text"
              max-width="200px"
            ></v-text-field>
          </v-col>
        </v-row>
      </v-layout>
    </v-card>
    <v-btn @click="nextView" depressed color="yellow">Next</v-btn>
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
