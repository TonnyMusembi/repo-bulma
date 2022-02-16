<template>
  <div class="about">
    <h1>This is an about page</h1>
  </div>
  <button v-on:click="openModal()">Open</button>
  <div class="modal" :class="{ 'is-active': open }">
    <div class="modal-background"></div>
    <div class="modal-card">
      <header class="modal-card-head">
        <p class="modal-card-title">Modal title</p>
        <button class="delete" aria-label="close"></button>
      </header>
      <section class="modal-card-body">
        <!-- Content ... -->
      </section>
      <footer class="modal-card-foot">
        <button class="button is-success" v-on:click="inGreet()">Save</button>
        <button class="button" v-on:click="onGreet()">Cancel</button>
      </footer>
    </div>
  </div>
  <div col="col-10">
    <button class="primary is-primary" v-on:click="loginOn()">Login</button>
  </div>
</template>
<script>
import Footer from "@/views/Footer";
export default {
  computed: {
    Footer,
  },
  data() {
    return {
      open: false,
    };
  },
  methods: {
    openModal() {
      this.open = true;
    },
    onGreet() {
      this.open = false;
    },
    inGreet() {
      this.open = true;
      // fetch().then((response) => {
      //   console.log(response).catch((error) => {
      //     console.log(error);
      //   });
      // });
    },
    loginOn() {
      this.open = true;
    },
  },
};
</script>
