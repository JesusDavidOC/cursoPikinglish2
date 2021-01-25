<template>
  <b-container fluid>
    <b-row>
      <b-col></b-col>
      <b-col sm="auto">
        <h3 class="titulo">HOW TO USE THE SUFFIX “ED”.</h3>
      </b-col>
      <b-col></b-col>
    </b-row>
    <b-row class="diamondContainer">
      <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
      <b-col>
        <h3 class="fuenteDiamond">
          The regular verbs in past tense are modified by adding “ed” as long as
          the sentence is affirmative.
        </h3>
      </b-col>
    </b-row>
    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="10">
        <tablaTC id="tabla1P8" :cuestionario="tabla1P8" />
      </b-col>
    </b-row>
    <b-row class="diamondContainer">
      <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
      <b-col>
        <h3 class="fuenteDiamond">
          Complete with the most suitable verb in the past form.
        </h3>
      </b-col>
    </b-row>
    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="10">
        <tablaTC id="" :cuestionario="tablaCompleteP8" />
      </b-col>
    </b-row>
    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="10">
        <tablaTC :cuestionario="tabla2P7" />
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
      <b-col sm="11">
        <tablaTC :cuestionario="tabla3P7" />
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
    opcionMultiple,
  },
  data() {
    return {
      tablaCompleteP8: {
        fields: [
          { key: "a", thClass: "noHead" },
          { key: "b", thClass: "noHead" },
          { key: "c", thClass: "noHead" },
          { key: "d", thClass: "noHead" },
          { key: "e", thClass: "noHead" },
          { key: "f", thClass: "noHead" },
          { key: "g", thClass: "noHead" },
        ],
        items:[
            {a:"Study", b: "Apply", c: "Try", d:"Cry", e:"Reply", f:"Dry", g:"Copy"}
        ]
      },
      tabla1P8: {
        fields: [
          {
            key: "a",
            label:
              "Verbs ending in “Y” preceded by a consonant are changed the “Y” to “I” + “ed” ",
          },
          { key: "b", label: "Verbs ending in “e” are just added the “d” " },
          { key: "c", label: "One syllable, double the last consonant" },
          { key: "d", label: "The rest of the verbs are added “ed” " },
        ],
        items: [
          {
            a: "Study - studied",
            b: "Love - loved",
            c: "Plan - planned",
            d: "Work - worked",
          },
          {
            a: "Apply - applied",
            b: "Sue-sued",
            c: "Mop-mopped",
            d: "Finish-finished",
          },
          {
            a: "Try-tried",
            b: "Like-liked",
            c: "Rub-rubbed",
            d: "Walk-walked ",
          },
          {
            a: "Cry-cried",
            b: "Tie-tied",
            c: "Stop-stopped Sob-sobbed",
            d: "Cook-cooked",
          },
          {
            a: "Reply- replied",
            b: "Breathe-breathed ",
            c: "",
            d: "Paint-painted",
          },
        ],
      },
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
              tamano: 18,
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
              tamano: 18,
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
              tamano: 20,
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
              tamano: 22,
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
              tamano: 15,
            },
          },
          {
            a: "I go for a run every morning",
            b: "Yo voy a correr cada mañana",
            complejo1: {
              lista: ["goes"],
              conTexto: true,
              textoA: "Karen",
              textoD: "for a run every morning ",
              tamano: 27,
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
              tamano: 22,
            },
          },
          {
            a: "You know me very well",
            b: "Tú me conoces muy bien",
            complejo1: {
              lista: ["knows"],
              conTexto: true,
              textoA: "That person",
              textoD: "me very well ",
              tamano: 25,
            },
          },
          {
            a: "I have something to tell you ",
            b: "Tengo algo que contarte ",
            complejo1: {
              lista: ["has"],
              conTexto: true,
              textoA: "She",
              textoD: "something to tell you",
              tamano: 23,
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
              tamano: 17,
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
              tamano: 14,
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
    };
  },
};
</script>

<style scoped>
/deep/ #tabla1P8 td {
  text-align: center !important;
}
</style>