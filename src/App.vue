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
@import url("https://fonts.googleapis.com/css2?family=Noto+Sans+TC:wght@100&display=swap");
@import "./assets/reset.css";

#app {
  font-family: "Noto Sans TC", sans-serif;
  background-color: black;
  height: 100vh;
}
</style>
