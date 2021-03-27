<template>
  <div id="nav">
    <div class="menu-item">
      <router-link to="/github">Github</router-link>
    </div>
    <div class="menu-item">
      <router-link to="/work">Work</router-link>
    </div>
    <div class="menu-item menu-center">
      <router-link to="/">NONO</router-link>
    </div>
    <div class="menu-item">
      <router-link to="/about">About</router-link>
    </div>
    <div class="menu-item">
      <router-link to="/about">Resume</router-link>
    </div>
  </div>
</template>

<script>
export default {
  name: "Navbar",
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Train+One&display=swap");
#nav {
  position: fixed;
  width: 100%;
  z-index: 2;
  left: 0;
  top: 0;
  padding: 30px;
  display: flex;
  align-items: center;
  justify-content: space-around;
  background-color: rgba(0, 0, 0, 0.3);
}
.menu-item a {
  font-weight: bold;
  font-size: 20px;
  color: #fff;
  text-decoration: none;
}
.menu-item a.router-link-exact-active,
.menu-item a:hover {
  color: #f0e8de;
  opacity: 0.6;
}
.menu-center a {
  font-size: 36px;
  font-family: "Train One", cursive;
}
</style>
