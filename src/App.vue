<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/login">Login</router-link>
    </div>
    <router-view/>
  </div>
</template>

<style lang="scss">

* {
  box-sizing: border-box;
}

body {
  background: linear-gradient(to bottom, #68EACC 0%, #497BE8 100%);
  min-height: 100vh;
  display: flex;
  font-weight: 400;
}

body,
html {
  width: 100%;
  height: 100%;
}

#app {
  position: relative;
  width: 100%;
  height: 100%;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;

}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;
  
    &.router-link-exact-active {
      color: #497BE8;
      text-decoration:none;
    }
  }
}

</style>
