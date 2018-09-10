<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <a href="https://medium.com/ethics-and-professional-issues-marcus-schimizzi">Blog</a>
    </div>
    <router-view/>
  </div>
</template>

<style lang="scss">
#app {
  // font-family: 'Roboto Mono', monospace;
  font-family: 'Poppins', sans-serif;
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
      color: #42b983;
    }
  }
}
.section-title {
  font-size: 4.5em;
}
</style>
