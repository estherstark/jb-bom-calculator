<script setup lang="js">

import Vue from "vue"
import Vuex from "vuex"

Vue.use(Vuex)

export default new Vuex.Store({
  state: {
    inputJob: "",
    inputSet: "",
    
  },
  mutations: {
    setInput1 (state, value) {
      state.input1 = value
    },
    setInput2 (state, value) {
      state.input2 = value
    }
  },
  actions: {
    setInput1 ({ commit }, value) {
      commit("setInput1", value)
    },
    setInput2 ({ commit }, value) {
      commit("setInput2", value)
    }
  },
  getters:{
    getResult: state => {
      return state.input1 + state.input2
    }
  }
})