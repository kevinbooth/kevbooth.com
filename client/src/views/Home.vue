<template>
  <div class="home container">
    <div class="row profile">
      <div class="three columns">
        <img src="@/assets/kevin.jpg" />
      </div>
      <div class="nine columns">
        <div class="vue-typer__container--home">
          <vue-typer 
            class="vue-typer--large"
            :text="typer" 
            erase-style="backspace"
            :erase-delay=50
          ></vue-typer>
        </div>
        <div class="follow unicon--inverse">
          <h1>Let's connect!</h1>
          <a href="https://www.linkedin.com/in/kevbooth" target="_blank"><unicon name="linkedin" width="30" height="30"></unicon></a>
          <a href="https://www.instagram.com/kevinbooth/" target="_blank"><unicon name="instagram" width="30" height="30"></unicon></a>
          <a href="https://www.facebook.com/KevinBoothh" target="_blank"><unicon name="facebook" width="30" height="30"></unicon></a>
        </div>
      </div>
    </div>
    <div class="row">
      <contact-form v-bind:class="{ visible: showForm }"></contact-form>
      <button 
        v-show="!showForm" 
        v-on:click="showForm = !showForm" 
        class="button--secondary"
      >Contact Me</button>
      </div>
  </div>
</template>

<script>
// @ is an alias to /src
import { VueTyper } from 'vue-typer'
import ContactForm from '@/components/ContactForm.vue'
import { SITE_NAME } from '@/variables.js'

export default {
  name: 'home',
  components: {
    VueTyper,
    ContactForm
  },
  data() {
    return {
      typer: ["Hi, I'm Kevin!", "And I'm a fullstack web developer!"],
      showForm: false
    }
  },
  metaInfo: {
    title: 'Home',
    titleTemplate: '%s - ' + SITE_NAME,
    htmlAttrs: {
      lang: 'en',
      amp: true
    }
  }
}
</script>

<style lang="scss">
.visible {
  max-height: 50rem !important;
}
</style>
