<template>
  <b-container fluid>
    <b-row>
      <b-col></b-col>
      <b-col sm="auto">
        <h3 class="titulo">PRESENT VERBS WITH THE 3RD SINGULAR PERSON.</h3>
      </b-col>
      <b-col></b-col>
    </b-row>
    <b-row class="diamondContainer">
      <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
      <b-col>
        <h3 class="fuenteDiamond">
          If the phrase is present, affirmative and it is conjugated by she, he
          and it then the verbs are added the “S, ES, S or Has to have”
        </h3>
      </b-col>
    </b-row>
    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="auto">
        <tablaTC id="tabla1P8" :cuestionario="tabla1P7" />
      </b-col>
    </b-row>
    <b-row class="diamondContainer">
      <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
      <b-col>
        <h3 class="fuenteDiamond">Rules to add the S, ES, IES</h3>
      </b-col>
    </b-row>
    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="10">
        <tablaTC id="tabla2P8" :cuestionario="tabla2P7" />
      </b-col>
    </b-row>
    <b-row class="diamondContainer">
      <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
      <b-col>
        <h3 class="fuenteDiamond">
          Rewrite the sentence, change the subject and modify the verb.
        </h3>
      </b-col>
    </b-row>
    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="10">
        <tablaTC id="tabla3P8" :cuestionario="tabla3P7" />
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
export default {
  components: {
    tablaTC,
  },
  data() {
    return {
      tabla3P7: {
        bordered: false,
        fields: [
          { key: "a", label: "I, you, we and they + verb" },
          { key: "b", label: "Spanish translation" },
          { key: "complejo1", label: "3rd singular person + verb (present)" },
        ],
        items: [
          {
            a: "They deny the truth",
            b: "Ellos niegan la verdad ",
            complejo1: {
              lista: ["ies"],
              conTexto: true,
              textoA: "She den",
              textoD: "the truth",
              tamano: 22,
              resuelto: true,
            },
          },
          {
            a: "We have to pay the bill",
            b: "Tenemos que pagar la cuenta",
            complejo1: {
              lista: ["has"],
              conTexto: true,
              textoA: "He",
              textoD: "to pay the bill",
              tamano: 22,
            },
          },
          {
            a: "They fix cars",
            b: "Ellos arreglan carros",
            complejo1: {
              lista: ["fixes"],
              conTexto: true,
              textoA: "The mechanic",
              textoD: "cars",
              tamano: 24,
            },
          },
          {
            a: "I neglect my loved ones",
            b: "Yo descuido mis seres queridos",
            complejo1: {
              lista: ["neglects"],
              conTexto: true,
              textoA: "She",
              textoD: "her loved ones",
              tamano: 26,
            },
          },
          {
            a: "We miss you",
            b: "Nosotros te extrañamos",
            complejo1: {
              lista: ["misses"],
              conTexto: true,
              textoA: "He",
              textoD: "you",
              tamano: 17,
            },
          },
          {
            a: "I go for a run every morning",
            b: "Yo voy a correr cada mañana",
            complejo1: {
              lista: ["goes"],
              conTexto: true,
              textoA: "Karen",
              textoD: "for a run",
              textoD2: " every morning",
              tamano: 21,
            },
          },
          {
            a: "They easily dismiss anyone",
            b: "Ellos despiden a cualquiera fácilmente",
            complejo1: {
              lista: ["dismisses"],
              conTexto: true,
              textoA: "He",
              textoD: "anyone easily.",
              tamano: 26,
            },
          },
          {
            a: "You know me very well",
            b: "Tú me conoces muy bien",
            complejo1: {
              lista: ["knows"],
              conTexto: true,
              textoA: "That person",
              textoD: "me very ",
              textoD2: "well",
              tamano: 26,
            },
          },
          {
            a: "I have something to tell you ",
            b: "Tengo algo que contarte ",
            complejo1: {
              lista: ["has"],
              conTexto: true,
              textoA: "She",
              textoD: "something",
              textoD2: "to tell you",
              tamano: 21,
            },
          },
          {
            a: "I walk every day",
            b: "Yo camino todos los días",
            complejo1: {
              lista: ["walks"],
              conTexto: true,
              textoA: "He",
              textoD: "every day",
              tamano: 21,
            },
          },
          {
            a: "You cry a lot",
            b: "Tú lloras mucho",
            complejo1: {
              lista: ["cries"],
              conTexto: true,
              textoA: "She",
              textoD: "a lot",
              tamano: 17,
            },
          },
        ],
      },
      tabla2P7: {
        fields: [
          { key: "a", label: "ES" },
          { key: "b", label: "IES" },
          { key: "c", label: "S" },
          { key: "d", label: "HAVE" },
        ],
        items: [
          {
            a: "Verbs ending in o, x, s, sh, ch, z",
            b:
              "If a verb ends with a consonant before -Y, we remove the y and add -IES",
            c: "Add an “S” to the rest of the verbs",
            d: "Has",
          },
        ],
      },
      tabla1P7: {
        fields: [
          { key: "a", label: "Present - I, you, they, we" },
          { key: "b", label: "Present - She, he, it" },
          { key: "c", label: "Past" },
          { key: "d", label: "Participle" },
          { key: "e", label: "Progressive" },
        ],
        items: [{ a: "SEE", b: "SEES", c: "Saw", d: "Seen", e: "Seeing" }],
      },
    };
  },
};
</script>

<style>
</style>