<template>
  <div class="home container">
    <div class="profile">
      <img src="@/assets/kevin.jpg" />
    </div>
    <div class="vue-typer__container">
      <vue-typer 
        class="vue-typer--large"
        :text="typer" 
        erase-style="backspace"
        :erase-delay=50
      ></vue-typer>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import { VueTyper } from 'vue-typer'

export default {
  name: 'home',
  components: {
    VueTyper
  },
  data() {
    return {
      typer: ["Hi, my name's Kevin Booth!", "And I'm a fullstack web developer!"]
    }
  },
}
</script>

