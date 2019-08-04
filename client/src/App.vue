<template>
  <div id="app">
    <div class="container">
      <div class="nav unicon">
        <a href="https://github.com/kevinbooth" target="_blank"><unicon name="github" width="30" height="30"></unicon></a>
        <a href="https://www.linkedin.com/in/kevbooth" target="_blank"><unicon name="linkedin" width="30" height="30"></unicon></a>
        <a href="https://www.instagram.com/kevinbooth/" target="_blank"><unicon name="instagram" width="30" height="30"></unicon></a>
        <a href="https://www.facebook.com/KevinBoothh" target="_blank"><unicon name="facebook" width="30" height="30"></unicon></a>
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
