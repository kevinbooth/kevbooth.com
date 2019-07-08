<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">home</router-link> |
      <router-link to="/about">about</router-link>
    </div>
    <router-view/>
  </div>
</template>

<style>
body {
  background-color: #031329;
  color: #80ffc6 !important;
  font-family: monospace !important;
}

#app {
  padding-top: 1rem;
  text-align: center;
}

#nav {
  padding-bottom: 2rem;
}
</style>
