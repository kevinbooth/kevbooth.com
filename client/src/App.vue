<template>
  <div id="app">
    <glowbar></glowbar>
    <div id="nav">
      <router-link to="/">home</router-link> |
      <router-link to="/about">about</router-link>
    </div>
    <router-view/>
  </div>
</template>

<script>
import Glowbar from '@/components/Glowbar.vue'

export default {
  components: {
    Glowbar
  }
}
</script>


<style>
body {
  background-color: #031329;
  color: #80ffc6 !important;
  font-family: monospace !important;
	background: linear-gradient(-45deg, #031329, #0f061d, #003244, #0b4033);
	background-size: 400% 400%;
	-webkit-animation: body-animate 15s infinite;
	-moz-animation: body-animate 15s infinite;
	animation: body-animate 15s infinite;
}

@-webkit-keyframes body-animate {
    0%{background-position:0% 50%}
    50%{background-position:100% 50%}
    100%{background-position:0% 50%}
}

@-moz-keyframes body-animate {
    0%{background-position:0% 50%}
    50%{background-position:100% 50%}
    100%{background-position:0% 50%}
}

@keyframes body-animate {
    0%{background-position:0% 50%}
    50%{background-position:100% 50%}
    100%{background-position:0% 50%}
}

#app {
  text-align: center;
}

#nav {
  padding-bottom: 2rem;
}
</style>
