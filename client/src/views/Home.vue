<template>
  <div class="home container">
    <div class="profile">
      <img src="@/assets/kevin.jpg" />
    </div>
    <HelloWorld msg="kevin booth"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'home',
  components: {
    HelloWorld
  }
}
</script>

<style lang="scss">
.profile {
  padding: 2rem 0;

  img {
    max-width: 14rem;
    border-radius: 100%;
    border: 3px solid #80ffc6;
  }
}
</style>

