<template>
  <b-container fluid>
    <b-row>
      <b-col></b-col>
      <b-col sm="auto">
        <h3 class="titulo">HOW TO USE THE SUFFIX “ED”.</h3>
      </b-col>
      <b-col></b-col>
    </b-row>
    <b-row>
      <b-col></b-col>
      <b-col sm="8">
        <p class="parrafo">
          As we know there are a lot of English irregular verbs that have a
          different spelling form in the past tense as well as in participle,
          however we have listed them in groups.
        </p>
      </b-col>
      <b-col></b-col>
    </b-row>
    <b-row class="diamondContainer">
      <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
      <b-col>
        <h3 class="fuenteDiamond">
          First group: Written the same way in all tenses.
        </h3>
      </b-col>
    </b-row>
    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="auto">
        <tablaTC id="tabla1P11" :cuestionario="tabla1P11" />
      </b-col>
    </b-row>
    <b-row class="diamondContainer">
      <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
      <b-col>
        <h3 class="fuenteDiamond">
          Second group. Ending in <span class="colorLetraRojo">GHT</span> in the
          past and as well as in participle.
        </h3>
      </b-col>
    </b-row>
    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="auto">
        <tablaTC id="tabla1P11" :cuestionario="tabla1P12" />
      </b-col>
    </b-row>
    <b-row class="diamondContainer">
      <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
      <b-col>
        <h3 class="fuenteDiamond">
          Third group: Those ending in <span class="colorLetraRojo">EN</span>
          in the participle form.
        </h3>
      </b-col>
    </b-row>
    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="auto">
        <tablaTC id="tabla1P11" :cuestionario="tabla2P12" />
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
import posiblesRespuestasTabla from "./posiblesRespuestasTabla";
import opcionMultiple from "./opcionMultiple";
import listaIndex from "./listaIndex";
import inputChecked from "./inputChecked";
import tablaTC from "./tablaTraduccionCodigos";
import audioComp from "./audioComp";
export default {
  components: {
    tablaTC,
    opcionMultiple,
    inputChecked,
    audioComp,
  },
  data() {
    return {
      tabla2P12: {
        fields: [
          { key: "a", label: "Present", thClass: "colorLetraRojo" },
          { key: "b", label: "Past", thClass: "colorLetraRojo" },
          { key: "html2", label: "Participle ", thClass: "colorLetraRojo" },
          { key: "d", label: "Translation ", thClass: "colorLetraRojo" },
        ],
        items: [
          {
            a: "Hide",
            b: "Hid",
            d: "Esconder, esconderse",
            html2: "<span class='colorLetraAzul'>Hidd<span class='colorLetraRojo'>en",
          },
          {
            a: "Bite",
            b: "Bit",
            d: "Morder.",
            html2: "<span class='colorLetraAzul'>Bitt<span class='colorLetraRojo'>en",
          },
          {
            a: "Drive",
            b: "Drove",
            d: "Conducir.",
            html2: "<span class='colorLetraAzul'>Driv<span class='colorLetraRojo'>en",
          },
          {
            a: "Write",
            b: "Wrote",
            d: "Escribir.",
            html2: "<span class='colorLetraAzul'>Writt<span class='colorLetraRojo'>en",
          },
          {
            a: "Ride",
            b: "Rode",
            d: "Subir.",
            html2: "<span class='colorLetraAzul'>Rid<span class='colorLetraRojo'>en",
          },
          {
            a: "Rise",
            b: "Rose",
            d: "Montar.",
            html2: "<span class='colorLetraAzul'>Ris<span class='colorLetraRojo'>en",
          },          
          {
            a: "Take",
            b: "Took",
            d: "Llevar o tomar.",
            html2: "<span class='colorLetraAzul'>Tak<span class='colorLetraRojo'>en",
          },
          {
            a: "See",
            b: "Saw",
            d: "Ver.",
            html2: "<span class='colorLetraAzul'>Se<span class='colorLetraRojo'>en",
          },
          {
            a: "Eat",
            b: "Ate",
            d: "Comer.",
            html2: "<span class='colorLetraAzul'>Eat<span class='colorLetraRojo'>en",
          },
          {
            a: "Wake",
            b: "Woke",
            d: "Despertar.",
            html2: "<span class='colorLetraAzul'>Wok<span class='colorLetraRojo'>en",
          },
          {
            a: "Speak",
            b: "Spoke",
            d: "Hablar.",
            html2: "<span class='colorLetraAzul'>Spok<span class='colorLetraRojo'>en",
          },
          {
            a: "Break",
            b: "Broke",
            d: "Romper.",
            html2: "<span class='colorLetraAzul'>Brok<span class='colorLetraRojo'>en",
          },
          {
            a: "Freeze",
            b: "Froze",
            d: "Congelar.",
            html2: "<span class='colorLetraAzul'>Froz<span class='colorLetraRojo'>en",
          },
          {
            a: "Shake",
            b: "Shook",
            d: "Sacudir.",
            html2: "<span class='colorLetraAzul'>Shak<span class='colorLetraRojo'>en",
          },
          {
            a: "Forget",
            b: "Forgot",
            d: "Olvidar.",
            html2: "<span class='colorLetraAzul'>Forgott<span class='colorLetraRojo'>en",
          },
          {
            a: "Steal",
            b: "Stole",
            d: "Robar.",
            html2: "<span class='colorLetraAzul'>Stol<span class='colorLetraRojo'>en",
          },
          {
            a: "Choose",
            b: "Chose",
            d: "Elegir.",
            html2: "<span class='colorLetraAzul'>Chos<span class='colorLetraRojo'>en",
          },
          {
            a: "Give",
            b: "Gave",
            d: "Dar.",
            html2: "<span class='colorLetraAzul'>Giv<span class='colorLetraRojo'>en",
          },
          {
            a: "Forgive",
            b: "Forgave",
            d: "Olvidar.",
            html2: "<span class='colorLetraAzul'>Forgiv<span class='colorLetraRojo'>en",
          },
          {
            a: "Forbid",
            b: "Forbade",
            d: "Prohibir.",
            html2: "<span class='colorLetraAzul'>Forbidd<span class='colorLetraRojo'>en",
          },
          {
            a: "Fall",
            b: "Fell",
            d: "Caer.",
            html2: "<span class='colorLetraAzul'>Fall<span class='colorLetraRojo'>en",
          },
          
        ],
      },
      tabla1P12: {
        fields: [
          { key: "a", label: "Present", thClass: "colorLetraRojo" },
          { key: "html1", label: "Past", thClass: "colorLetraRojo" },
          { key: "html2", label: "Participle ", thClass: "colorLetraRojo" },
          { key: "d", label: "Translation ", thClass: "colorLetraRojo" },
        ],
        items: [
          {
            a: "Buy",
            html1: "Bou<span class='colorLetraRojo'>ght",
            html2: "Bou<span class='colorLetraRojo'>ght",
            d: "Comprar.",
          },
          {
            a: "Think",
            html1: "Thou<span class='colorLetraRojo'>ght",
            html2: "Thou<span class='colorLetraRojo'>ght",
            d: "Pensar.",
          },
          {
            a: "Catch",
            html1: "Cau<span class='colorLetraRojo'>ght",
            html2: "Cau<span class='colorLetraRojo'>ght",
            d: "Atrapar.",
          },
          {
            a: "Teach",
            html1: "Tau<span class='colorLetraRojo'>ght",
            html2: "Tau<span class='colorLetraRojo'>ght",
            d: "Enseñar.",
          },
          {
            a: "Bring",
            html1: "Brou<span class='colorLetraRojo'>ght",
            html2: "Brou<span class='colorLetraRojo'>ght",
            d: "Traer.",
          },
          {
            a: "Fight",
            html1: "Fou<span class='colorLetraRojo'>ght",
            html2: "Fou<span class='colorLetraRojo'>ght",
            d: "Pelear.",
          },
        ],
      },
      tabla1P11: {
        fields: [
          { key: "a", label: "Present", thClass: "colorLetraRojo" },
          { key: "b", label: "Past", thClass: "colorLetraRojo" },
          { key: "c", label: "Participle ", thClass: "colorLetraRojo" },
          { key: "d", label: "Translation ", thClass: "colorLetraRojo" },
        ],
        items: [
          {
            a: "Set",
            b: "Set",
            c: "Set",
            d: "Configurar, ajustar, programar, organizar.",
          },
          { a: "Let", b: "Let", c: "Let", d: "Permitir, dejar." },
          { a: "Cut", b: "Cut", c: "Cut", d: "Cortar." },
          { a: "Put", b: "Put", c: "Put", d: "Poner." },
          { a: "Hit", b: "Hit", c: "Hit", d: "Golpear." },
          { a: "Hurt", b: "Hurt", c: "Hurt", d: "Lastimar." },
          { a: "Broadcast", b: "Broadcast", c: "Broadcast", d: "Transmitir." },
          { a: "Bet", b: "Bet", c: "Bet", d: "Apostar." },
          { a: "Shut", b: "Shut", c: "Shut", d: "Cerrar." },
          { a: "Read", b: "Read", c: "Read", d: "Leer." },
          { a: "Spread", b: "Spread", c: "Spread", d: "Extender." },
          { a: "Quit", b: "Quit", c: "Quit", d: "Renunciar a." },
          { a: "Burst", b: "Burst", c: "Burst", d: "Estallar." },
          { a: "Cost", b: "Cost", c: "Cost", d: "Costar." },
          { a: "Shed", b: "Shed", c: "Shed", d: "Perder la piel." },
        ],
      },
    };
  },
};
</script>

<style scoped>
</style>