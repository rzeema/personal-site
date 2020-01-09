<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link> |
      <router-link to="/projects">Projects</router-link> |
      <router-link to="/fun">Fun</router-link>
    </div>
    <router-view />
  </div>
</template>

<style lang="scss">
$bk-color: #3a3b3b;
body {
  background-color: $bk-color;
}

#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #c6c3bd;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #c6c3bd;

    &.router-link-exact-active {
      color: #ebe9e6;
    }
  }
}
</style>
