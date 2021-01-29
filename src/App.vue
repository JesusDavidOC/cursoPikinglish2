<template>
  <div id="app">
    <leccion1 />
  </div>
</template>

<script>
import app from "./assets/app.css";
import leccion1 from "./components/curso2P49";
export default {
  name: "App",
  components: {
    leccion1,
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