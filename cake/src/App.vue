<template>
  <div id="app">
    <navbar></navbar>
    <router-view />
  </div>
</template>

<script>
/* eslint-disable */
import navbar from "@/components/Navbar.vue";
import Vue from "vue";
import Navbar from "./components/Navbar.vue";

Vue.component("navbar", navbar);
export default {
  components: { Navbar },
};
</script>
<style scoped>
html body {
  margin: 0px;
  padding: 0px;
}
</style>
