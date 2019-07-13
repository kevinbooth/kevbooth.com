<template>
  <div id="app">
    <div class="container">
      <div class="nav">
        <router-link to="/">home</router-link> |
        <router-link to="/skills">skills</router-link>
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
