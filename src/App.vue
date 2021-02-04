<template>
  <div id="app">
    <leccion1 />
    <leccion2 />
    <leccion3 />
    <leccion4 />
    <leccion5 />
    <leccion6 />
    <leccion7 />
    <leccion8 />
    <leccion9 />
  </div>
</template>

<script>
import app from "./assets/app.css";
import leccion1 from "./components/curso2Leccion1";
import leccion2 from "./components/curso2Pag82";
import leccion3 from "./components/curso2Pag84";
import leccion4 from "./components/curso2Pag88";
import leccion5 from "./components/curso2Pag91";
import leccion6 from "./components/curso2Pag94";
import leccion7 from "./components/curso2Pag102";
import leccion8 from "./components/curso2Pag106";
import leccion9 from "./components/curso2Pag113";
export default {
  name: "App",
  components: {
    leccion1,
    leccion2,
    leccion3,
    leccion4,
    leccion5,
    leccion6,
    leccion7,
    leccion8,
    leccion9,
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
