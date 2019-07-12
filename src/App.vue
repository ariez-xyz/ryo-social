<template>
  <div id="app">
    <div class="cookieDisclaimer" v-if="!disclaimerClicked">
      <p class="alert">DISCLAIMER</p>
      <p>This site uses cookies</p>
      <button v-on:click="disclaimerClicked = true">Go away</button>
    </div>

    <div id="nav">
      <router-link to="/"><b>Main</b></router-link> |
      <router-link to="/about"><b>FAQ</b></router-link> |
      <router-link to="/coc"><b>Verhaltenskodex</b></router-link> |
      <router-link to="/complaints"><b>Beschwerden</b></router-link>
    </div>

    <router-view/>

  </div>
</template>

<style>
  @import "https://fonts.googleapis.com/css?family=Montserrat:700,900&display=swap";
  @import "styles/main.css";
</style>

<script>
  export default {
    data: function () {
      return {
        disclaimerClicked: false
      }
    }
  }
</script>