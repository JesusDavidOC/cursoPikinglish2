<template>
  <div style="font-size: 1.3em">
    <div v-for="(option, index) in $props.options" class="row" :key="option.pregunta+index">
      <b-col sm="auto">
        <b-form-group
          :label="option.pregunta"
          :id="index + ''"
          label-size="xl"
          label-class="labelPregunta"
        >
          <b-form-radio-group
            :name="index + ''"
            :options="option.options"
            stacked
            @change="dmensaje($event, index)"
          >
          </b-form-radio-group> </b-form-group
      ></b-col>

      <b-col v-if="option.audio != undefined">
        <div class="input-group-append">
          <button          
            class="btn btn-outline-secondary"
            type="button"
            v-on:click="playSound(option.audio)"
          >
            <i class="fa fa-play"></i>
          </button>
        </div>
      </b-col>
    </div>
  </div>
</template>


<script>
export default {
  props: {
    options: Array,
    label: String,
    rEsperadas: Array,
  },
  data() {
    return {
      mensaje: "",
      Rrespuestas: [],
    };
  },
  methods: {
    enviar(checked) {
      this.$emit("RESULTADO", checked);
    },
    verificacion: function (respuestas, rEsperadas) {
      this.mensaje = "LAS RESPUESTAS A LAS PREGUNTAS: ";
      if (respuestas.length != rEsperadas.length) {
        this.mensaje = "DILIGENCIE TODAS LAS PREGUNTAS.";
      } else {
        for (var r = 0; r < respuestas.length; r++) {
          if (respuestas[r] != rEsperadas[r]) {
            if(r != respuestas.length-1){
              this.mensaje = this.mensaje + (r + 1) + "-";
            } else {
              this.mensaje = this.mensaje + (r + 1);
            }            
          }
        }
        this.mensaje = this.mensaje + " SON EQUIVOCADAS, REVISALAS DE NUEVO!"
      }
      if (this.mensaje == "LAS RESPUESTAS A LAS PREGUNTAS: ") {
        this.mensaje = "TODAS LAS RESPUESTAS CORRECTAS";
      }
      this.enviar(this.mensaje);
    },
    dmensaje(valor, posicion) {
      this.Rrespuestas[posicion] = valor;
      this.verificacion(this.Rrespuestas, this.rEsperadas);
    },
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
/deep/.labelPregunta {
  font-weight: bold;
}
.btn{
  margin-top: 1em;
  border-radius: 2em;
  height: 2em;
  width: 2em;
  font-size: 1.5em;
  padding-left: -0.4em;
  background-color: cornflowerblue;
  color: aliceblue;
}
</style>