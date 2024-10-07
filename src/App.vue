<template>
  <v-app>
    <v-main class="main">
      <HomePage />
    </v-main>
  </v-app>
</template>

<script setup>
import HomePage from "./components/HomePage.vue";
</script>
<style scoped>
.main {
  background-color: hsl(257, 40%, 49%);
  background-image: url("/src/assets/bg-desktop.svg"); /* Path to the image */
  background-size: cover; /* Ensures the image maintains its aspect ratio */
  background-position: center; /* Centers the image */
  background-repeat: no-repeat; /* Prevents the image from repeating */
  height: 100%; /* Sets the height of the main element to fill the viewport */
}
@media screen and (max-width: 599.5px) {
  /* Your CSS rules for screens 599.5px and below */
  .main {
    background-image: url("/src/assets/bg-mobile.svg"); /* Path to the image */
  }
}
</style>