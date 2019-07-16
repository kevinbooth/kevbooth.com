<template>
  <div id="app">
    <div class="container">
      <div class="nav unicon">
        <img src="@/assets/logo.svg" />
        <router-link to="/"><unicon name="home-alt" width="30" height="30"></unicon></router-link>
        <router-link to="/skills"><unicon name="screw" width="30" height="30"></unicon></router-link>
      </div>
      <glowbar></glowbar>
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
