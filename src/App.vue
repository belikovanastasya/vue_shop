<template>
  <div id="app">
    <nav>
      <div class="container">
        <ul class="nav__left">
          <!-- Navigation Links -->
          <li>
            <router-link to="/">Home</router-link>
          </li>
          <li>
            <router-link to="/admin">Admin</router-link>
          </li>
          <li>
            <router-link to="/cart">Cart</router-link>
          </li>
        </ul>
      </div>
    </nav>
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: "App"
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
<style lang="scss">
body {
  padding: 0;
  margin: 0;
  width: 100%;
}
.container {
  width: 100%;
  max-width: 1200px;
  margin: 0 auto;
}
.nav__left {
  margin: 0;
  width: 200px;
  display: flex;
  flex-direction: row;
  list-style: none;
  justify-content: space-between;
  align-items: center;
  text-transform: uppercase;
  height: 50px;
  background: yellow;
  padding: 0 15px;
  li a {
    text-decoration: none;
    color: #000;
  }
}
</style>
