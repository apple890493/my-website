<template>
  <div id="app">
    <Navbar />
    <router-view />
  </div>
</template>

<script>
import Navbar from "@/components/Navbar.vue";

export default {
  components: {
    Navbar,
  },
};
</script>

<style>
@import "./assets/reset.css";

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  background-color: black;
  height: 100vh;
}
</style>
