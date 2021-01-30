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
            d: "Comprar.",
            html2: "<span class='colorLetraAzul'>Hidd<span class='colorLetraRojo'>en",
          },
          {
            a: "Hide",
            b: "Hid",
            d: "Comprar.",
            html2: "<span class='colorLetraAzul'>Hidd<span class='colorLetraRojo'>en",
          },
          {
            a: "Hide",
            b: "Hid",
            d: "Comprar.",
            html2: "<span class='colorLetraAzul'>Hidd<span class='colorLetraRojo'>en",
          },
          {
            a: "Hide",
            b: "Hid",
            d: "Comprar.",
            html2: "<span class='colorLetraAzul'>Hidd<span class='colorLetraRojo'>en",
          },
          {
            a: "Hide",
            b: "Hid",
            d: "Comprar.",
            html2: "<span class='colorLetraAzul'>Hidd<span class='colorLetraRojo'>en",
          },
          {
            a: "Hide",
            b: "Hid",
            d: "Comprar.",
            html2: "<span class='colorLetraAzul'>Hidd<span class='colorLetraRojo'>en",
          },
          {
            a: "Hide",
            b: "Hid",
            d: "Comprar.",
            html2: "<span class='colorLetraAzul'>Hidd<span class='colorLetraRojo'>en",
          },
          {
            a: "Hide",
            b: "Hid",
            d: "Comprar.",
            html2: "<span class='colorLetraAzul'>Hidd<span class='colorLetraRojo'>en",
          },
          {
            a: "Hide",
            b: "Hid",
            d: "Comprar.",
            html2: "<span class='colorLetraAzul'>Hidd<span class='colorLetraRojo'>en",
          },
          {
            a: "Hide",
            b: "Hid",
            d: "Comprar.",
            html2: "<span class='colorLetraAzul'>Hidd<span class='colorLetraRojo'>en",
          },
          {
            a: "Hide",
            b: "Hid",
            d: "Comprar.",
            html2: "<span class='colorLetraAzul'>Hidd<span class='colorLetraRojo'>en",
          },
          {
            a: "Hide",
            b: "Hid",
            d: "Comprar.",
            html2: "<span class='colorLetraAzul'>Hidd<span class='colorLetraRojo'>en",
          },
          {
            a: "Hide",
            b: "Hid",
            d: "Comprar.",
            html2: "<span class='colorLetraAzul'>Hidd<span class='colorLetraRojo'>en",
          },
          {
            a: "Hide",
            b: "Hid",
            d: "Comprar.",
            html2: "<span class='colorLetraAzul'>Hidd<span class='colorLetraRojo'>en",
          },
          {
            a: "Hide",
            b: "Hid",
            d: "Comprar.",
            html2: "<span class='colorLetraAzul'>Hidd<span class='colorLetraRojo'>en",
          },
          {
            a: "Hide",
            b: "Hid",
            d: "Comprar.",
            html2: "<span class='colorLetraAzul'>Hidd<span class='colorLetraRojo'>en",
          },
          {
            a: "Hide",
            b: "Hid",
            d: "Comprar.",
            html2: "<span class='colorLetraAzul'>Hidd<span class='colorLetraRojo'>en",
          },
          {
            a: "Hide",
            b: "Hid",
            d: "Comprar.",
            html2: "<span class='colorLetraAzul'>Hidd<span class='colorLetraRojo'>en",
          },
          {
            a: "Hide",
            b: "Hid",
            d: "Comprar.",
            html2: "<span class='colorLetraAzul'>Hidd<span class='colorLetraRojo'>en",
          },
          {
            a: "Hide",
            b: "Hid",
            d: "Comprar.",
            html2: "<span class='colorLetraAzul'>Hidd<span class='colorLetraRojo'>en",
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