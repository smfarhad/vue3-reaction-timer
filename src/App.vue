<template>
  <div class="app">
    <h1>Ninja Reaction Timer</h1>
    <button @click="start">play</button>
  </div>
</template>
<script>
export default {
  name: "App",
  components: {},
  data() {
    isPlaying: false;
    delay: 0;
  },
  methods: {
    start() {
      this.delay = 2000+Math.random()*5000;
      this.isPlaying = true;
      console.log(this.delay);
    }
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #444;
  margin-top: 60px;
}
</style>
