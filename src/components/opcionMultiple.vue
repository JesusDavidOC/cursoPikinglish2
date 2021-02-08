<template>
  <b-container style="font-size: 1.3em">
    <b-row
      v-for="(option, index) in $props.object.options"
      :key="option.pregunta + index"
    >
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
            id="play"
            class="btn btn-outline-secondary"
            type="button"
            v-on:click="playSound(option.audio)"
          >
            <i class="fa fa-play"></i>
          </button>
        </div>
      </b-col>
    </b-row>
    <b-modal
      :ref="object.options[0].pregunta + object.options[0].options[0].text"
      hide-footer
      title="RESULTADO"
    >
      <h3 class="subTitulo" v-if="mensaje != ''">{{ mensaje }}</h3>
      <h3 class="subTitulo" v-if="mensaje == ''">
        POR FAVOR, COMPLETE LAS PREGUNTAS.
      </h3>
    </b-modal>
    <b-row>
      <b-col></b-col>
      <b-col sm="auto">
        <b-button
          variant="primary"
          @click="
            showModal(
              object.options[0].pregunta + object.options[0].options[0].text
            )
          "
          >VERIFICAR PREGUNTAS</b-button
        >
      </b-col>
      <b-col></b-col>
    </b-row>
  </b-container>
</template>


<script>
export default {
  props: {
    object: Object,
  },
  data() {
    return {
      mensaje: "",
      Rrespuestas: [],
    };
  },
  methods: {
    showModal(text) {
      this.$refs[text].show();
    },
    verificacion: function (respuestas, rEsperadas) {
      this.mensaje = "LAS RESPUESTAS A LAS PREGUNTAS: ";
      if (respuestas.length != rEsperadas.length) {
        this.mensaje = "DILIGENCIE TODAS LAS PREGUNTAS.";
      } else {
        for (var r = 0; r < respuestas.length; r++) {
          if (respuestas[r] != rEsperadas[r]) {
            if (r != 0) {
              this.mensaje = this.mensaje + "-" + (r + 1);
            } else {
              this.mensaje = this.mensaje + (r + 1);
            }
          }
        }
        this.mensaje = this.mensaje + " SON EQUIVOCADAS, REVISALAS DE NUEVO!";
      }
      if (
        this.mensaje ==
        "LAS RESPUESTAS A LAS PREGUNTAS: " +
          " SON EQUIVOCADAS, REVISALAS DE NUEVO!"
      ) {
        this.mensaje = "TODAS LAS RESPUESTAS CORRECTAS";
      }
    },
    dmensaje(valor, posicion) {
      this.Rrespuestas[posicion] = valor;
      this.verificacion(this.Rrespuestas, this.object.rEsperadas);
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
#play {
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