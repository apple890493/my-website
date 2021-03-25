<template>
  <div id="nav">
    <div class="menu-item">
      <router-link to="/">Home</router-link>
    </div>
    <div class="menu-item">
      <router-link to="/about">About</router-link>
    </div>
    <div class="menu-item">
      <router-link to="/about">About</router-link>
    </div>
  </div>
</template>

<script>
export default {
  name: "Navbar",
};
</script>

<style scoped>
#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #fff;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
