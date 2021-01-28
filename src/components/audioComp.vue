<template>
  <b-container fluid class="ic">
    <b-row :style="'width:'+elemento.tamano+'em;'">
      <b-col sm="auto" style="padding-right: 0" v-if="elemento.textoA != undefined">
        <p class="parrafoIC" v-html="elemento.textoA">{{ elemento.textoA }}</p>
      </b-col>
      <b-col sm="auto" id="audio">
        <button
          class="btn btn-outline-secondary"
          type="button"
          v-on:click="playSound(elemento.audio)"
        >
          <i class="fa fa-play"></i>
        </button>
      </b-col>
      <b-col sm="auto" style="padding-left: 0" v-if="elemento.textoB != undefined">
        <p class="parrafoIC" v-html="elemento.textoD">{{ elemento.textoD }}</p>
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
export default {
  props: {
    elemento: Object,
  },
  methods: {
    playSound(sound) {
      if (sound) {
        var audio = new Audio(sound);
        audio.play();
      }
    },
  },
};
</script>

<style scoped>
.btn {
  border-radius: 2em;
  height: 2em;
  width: 2em;
  font-size: 1em;
  text-align: center;
  background-color: cornflowerblue;
  color: aliceblue;
  padding: 0;
  
}

#audio{
    padding: 0.5em;
    padding-top:0em;
    padding-bottom: 0.1em;
    height: 80%;
}
</style>