<template>
  <div class="home">
    <img
      alt="background-tree"
      class="background"
      src="../assets/images/back-tree.jpg"
    />
    <img
      alt="foreground-tree"
      class="foreground"
      src="../assets/images/front-tree.png"
    />
    <div class="section section-one">
      <div class="text-content">
        <h1>Welcome Here!</h1>
      </div>
    </div>
    <div class="section section-sec">
      <div class="text-content">
        <h1>I am Nono</h1>
      </div>
    </div>
  </div>
</template>

<script>
// import Navbar from "@/components/Navbar.vue";

export default {
  name: "Home",
  components: {
    // Navbar,
  },
};
</script>

<style scoped>
img.background,
img.foreground {
  min-height: 100%;
  min-width: 100%;
  width: 100vw;
  height: 80vh;
}

img.background {
  position: fixed;
  top: 0;
  left: 0;
}

.section {
  min-height: 100vh;
  position: relative;
}
</style>
