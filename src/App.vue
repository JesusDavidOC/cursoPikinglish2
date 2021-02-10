<template>
  <div id="app">
    <leccion/>
  </div>
</template>

<script>
import app from "./assets/app.css";
import leccion from "./components/curso2P8"
export default {
  name: "App",
  components: {
    leccion
  },
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
  padding-left: 1em;
}
</style>
