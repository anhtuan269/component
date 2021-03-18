<template>
  <div class="container">
    <div class="row">
      <div class="col-sm-12">
        <button
          class="btn btn-outline-danger"
          @click="selectedComponent = 'appHome'"
        >
          Home
        </button>
        <button
          class="btn btn-outline-danger"
          @click="selectedComponent = 'appContact'"
        >
          Contact
        </button>
        <button
          class="btn btn-outline-danger"
          @click="selectedComponent = 'appAbout'"
        >
          About
        </button>
      </div>
    </div>
    <div class="row">
      <div class="col-sm-12">
          <component :is="selectedComponent"></component>
      </div>
    </div>
  </div>
</template>

<script>
import Home from "./components/Home.vue";
import Contact from "./components/Contact.vue";
import About from "./components/About.vue";

export default {
  name: "App",
  data() {
    return {
      selectedComponent: "appHome",
    };
  },
  components: {
    appHome: Home,
    appContact: Contact,
    appAbout: About,
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
#app .container .row {
  margin-top: 50px;
}
</style>
