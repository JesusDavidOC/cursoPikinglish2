<template>
  <b-container class="ic" fluid>
    <b-row :style="'width: ' + tamano + 'em;' +'display: inline-flex;'">
      <b-col v-if="conTexto && textoA != ''" sm="auto" style="padding-right: 0">
        <p class="parrafoIC" v-html="textoA">{{ textoA }}</p>
      </b-col>
      <b-col style="display: inline-flex; padding-left:0.5em; padding-right: 0.5em ">
        <b-form-input
          :name="this.name + esperado[0]"
          :id="this.name + esperado[0]"
          v-model="text"
          :state="this.contiene()"
          aria-describedby="input-live-help input-live-feedback"
          trim
          class="text"          
        ></b-form-input>
        <div class="input-group-append">
          <button
            id="noAudio"
            v-if="$props.audio == undefined"
            class="btn btn-outline-secondary"
            type="button"
            v-on:click="completar"
          >
            <i class="fa fa-eye"></i>
          </button>

          <button
            id="paraAudio"
            v-if="$props.audio != undefined"
            class="btn btn-outline-secondary"
            type="button"
            v-on:click="completar"
            style="border-radius: 0"
          >
            <i class="fa fa-eye"></i>
          </button>

          <button
            id="paraAudio"
            v-if="$props.audio != undefined"
            class="btn btn-outline-secondary"
            type="button"
            @click.prevent="playSound(audio)"
          >
            <i class="fa fa-play"></i>
          </button>
        </div>
      </b-col>
      <b-col v-if="conTexto && textoD != ''" sm="auto" style="padding-left: 0;padding-right: 0px">
          <p class="parrafoIC" v-html="textoD">{{ textoD }}</p>
      </b-col>
    </b-row>
    <b-row>
        <b-col v-if="conTexto" sm="auto" style="padding-left: 0">
          <p class="parrafoIC" v-html="textoD2">{{ textoD2 }}</p>
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
export default {
  props: {
    esperado: Array,
    resuelto: Boolean,
    name: "",
    conTexto: Boolean,
    textoA: String,
    textoD: String,
    textoD2: String,
    audio: "",
    tamano: Number,
  },
  data() {
    return {
      text: "",
      esperado1: this.esperado,
    };
  },
  methods: {
    playSound(sound) {
      if (sound) {
        var audio = new Audio(sound);
        audio.play();
      }
    },
    completar() {
      this.text = this.esperado[0];
    },
    quitarAcentos(cadena) {
      const acentos = {
        á: "a",
        é: "e",
        í: "i",
        ó: "o",
        ú: "u",
        Á: "A",
        É: "E",
        Í: "I",
        Ó: "O",
        Ú: "U",
      };
      return cadena
        .split("")
        .map((letra) => acentos[letra] || letra)
        .join("")
        .toString();
    },
    contiene() {
      //console.log(this.esperado1)
      this.text = this.text.replace("´", "'");
      if (
        this.esperado1.includes(this.quitarAcentos(this.text.toLowerCase()))
      ) {
        this.$emit("output", this.text);
        return true;
      }
      return false;
    },
  },
  mounted() {
    if (this.resuelto) {
      this.text = this.esperado1[0];
    }
    var nuevo2 = [];
    for (var i = 0; i < this.esperado1.length; i++) {
      nuevo2.push(
        this.quitarAcentos(this.esperado1[i]).toLowerCase().replace("´", "'")
      );
    }
    this.esperado1 = nuevo2;
  },
};
</script>

<style scoped>
#ic{
    height: 100%;
}
.input-group-append {
  height: 90%;
}
/deep/ .form-control{
  border-top-left-radius: 0.4em;
  border-bottom-left-radius: 0.4em;
  border-top-right-radius: 0em !important;
  border-bottom-right-radius: 0em !important;
  line-height: 1em;   
}
.text {
  font-size: 1.3em;
  
}
.btn{
    border-bottom-left-radius: 0em;
    border-top-left-radius: 0em;
    padding-top: 0.2em;
}

#paraAudio {
  width: 1.2em;
  padding-right: 0;
  padding-left: 0;
}
.form-control {
  padding-top: 0;
  height: 90%;
  padding-bottom: 0;
  padding-right: 0;
}

#noAudio {
  border-top-right-radius: 0.5em;
  border-bottom-right-radius: 0.5em;
}
</style>