/* eslint-disable */
<template>
  <div>
    <v-toolbar color="grey darken-4" dense dark>
      <v-appbar-nav-icon>
        <v-img :src="require('../assets/logo-jb.png')" />
      </v-appbar-nav-icon>
      <v-toolbar-title>JB BoM Calculator</v-toolbar-title>
    </v-toolbar>
    <v-form>
      <v-container>
        <v-row>
          <v-col cols="12" sm="6">
            <h1>Welcome to <br />JB BoM Calculator</h1>
            <v-img :src="require('../assets/img-login.png')" />
          </v-col>

          <v-col cols="12" sm="6">
            <v-text-field
              solo
              label="Append"
              append-icon="mdi-map-marker"
            ></v-text-field>
          </v-col>

          <v-col cols="12" sm="6">
            <v-card
              class="pa-md-4 mx-lg-auto"
              color="grey lighten-2"
              width="500px"
              elevation="1"
              text-center
              secondary
              text-no-wrap
              rounded-lg
            >
              <h2 class="text-subtitle-2 text-center">Please Log In</h2>

              <v-text-field
                label="Employee ID"
                outlined
                :rules="rules"
              ></v-text-field>
              <v-text-field
                label="Password"
                outlined
                :rules="rules"
              ></v-text-field>
              <v-btn class="login-btn" depressed color="yellow" accent-4>
                login
              </v-btn>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </v-form>
  </div>
</template>
