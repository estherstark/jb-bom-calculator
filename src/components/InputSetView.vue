<template>
  <v-app>
    <h1 class="ma-4 font-weight-regular text-center">
      Input Details to Calculate
    </h1>

    <v-card class="pa-4 ma-2 d-flex justify-center align-center">
      <v-layout column align-center>
        <v-row>
          <v-col class="order-2">
            <p>Job Name</p>
          </v-col>
          <v-col><v-text-field outlined></v-text-field> </v-col>
        </v-row>

        <v-row>
          <v-col class="order-1">
            <p>Number of Set</p>
          </v-col>
          <v-col><v-text-field outlined></v-text-field> </v-col>
        </v-row>

        <v-col> <v-btn>Next</v-btn></v-col>
      </v-layout>
    </v-card>
  </v-app>
</template>

<script>
export default {
  name: "InputSetView",
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
</style>
