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
    <contact-form v-bind:class="{ visible: !showForm }"></contact-form>
    <button 
      v-show="!showForm" 
      v-on:click="showForm = !showForm" 
      class="button--secondary"
    >Contact Me</button>
  </div>
</template>

<script>
// @ is an alias to /src
import { VueTyper } from 'vue-typer'
import ContactForm from '@/components/ContactForm.vue'

export default {
  name: 'home',
  components: {
    VueTyper,
    ContactForm
  },
  data() {
    return {
      typer: ["Hi, my name's Kevin Booth!", "And I'm a fullstack web developer!"],
      showForm: false
    }
  },
}
</script>

<style lang="scss">
.visible {
  visibility: hidden;
}
</style>
