<template>
  <div class="home">
    <!-- <img alt="Vue logo" src="../assets/logo.png" /> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App" /> -->
  </div>
  <div class="primary button">Home</div>
  <button class="button primary" v-on:click="Greet()">Add New Vehicle</button>
  <button class="button is-dark">Load</button>
  <div class="col-4">
    <div class="container">
      <div class="notification is-primary">
        This container is <strong>centered</strong> on desktop and larger
        viewports.
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
//import HelloWorld from "@/components/HelloWorld.vue";
//import Footer from '@/views/Footer'
export default {
  name: "Home",
  components: {
    // HelloWorld,
    //Footer,
  },
};
</script>
