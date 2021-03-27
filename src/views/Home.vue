<template>
  <div class="home">
    <div class="zoom">
      <img
        alt="background-tree"
        class="background"
        :style="{ transform: `scale(${offSet}, ${offSet})` }"
        src="../assets/images/back-tree.jpg"
      />
    </div>

    <div class="section section-one">
      <h1 class="first-text">Welcome Here</h1>
    </div>
  </div>
</template>

<script>
export default {
  name: "Home",
  data() {
    return {
      setWidth: 1,
    };
  },
  created() {
    window.addEventListener("scroll", this.handleScroll);
  },
  methods: {
    handleScroll() {
      let scroll = window.scrollY;
      this.setWidth = 1 + scroll / 1000;
      console.log(scroll / 100);
    },
  },
  computed: {
    offSet() {
      return this.setWidth;
    },
  },
};
</script>

<style scoped>
.home {
  overflow: scroll;
}
.zoom {
  position: relative;
  width: 100vw;
  height: 200vh;
}

img.background {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}

.section {
  z-index: 2;
  position: fixed;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  text-align: center;
  color: #fff;
}
</style>
