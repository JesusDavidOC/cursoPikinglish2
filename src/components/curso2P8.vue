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
        <tablaTC :cuestionario="tablaCompleteP9" />
      </b-col>
    </b-row>
    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="11">
        <b-row
          v-for="(item, index) in listadoCompletarP9"
          :key="index + item.textoA"
          class="margin-bottom"
        >
          <b-col
            ><inputChecked
              :esperado="item.listado"
              :conTexto="true"
              :textoA="item.textoA"
              :textoD="item.textoD"
              :tamano="item.tamano"
              :textoD2="item.textoD2"
          /></b-col>
        </b-row>
      </b-col>
    </b-row>
    <b-row>
      <b-col>
        <h3 class="subTitulo">HOW TO PRONOUNCE THE SUFFIX “ED”</h3>
      </b-col>
    </b-row>
    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="3">
        <b-row>
          <b-col>
            <h3 class="subTitulo">Ending sounds</h3>
          </b-col>
        </b-row>
        <b-row class="diamondContainer">
          <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
          <b-col>
            <h3 class="fuenteDiamond">N, L, M, Y, R, U, V, B, G, Z.</h3>
          </b-col>
        </b-row>
        <b-row class="diamondContainer">
          <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
          <b-col>
            <h3 class="fuenteDiamond">
              some consonants sound differently from Spanish sounds such as:
              clo<strong>se: Z</strong>
            </h3>
          </b-col>
        </b-row>
        <b-row class="diamondContainer">
          <b-col>
            <h3 class="fuenteDiamond">SOUND: “d”</h3>
          </b-col>
        </b-row>
      </b-col>
      <b-col sm="7">
        <tablaTC :cuestionario="tabla1P10" />
      </b-col>
    </b-row>
    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="3">
        <b-row>
          <b-col>
            <h3 class="subTitulo">Ending sounds</h3>
          </b-col>
        </b-row>
        <b-row class="diamondContainer">
          <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
          <b-col>
            <h3 class="fuenteDiamond">K, F, SH, S, X, P.</h3>
          </b-col>
        </b-row>
        <b-row class="diamondContainer">
          <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
          <b-col>
            <h3 class="fuenteDiamond">
              some consonants sound differently from Spanish sounds such as:
              Lau<strong>gh: F</strong>
            </h3>
          </b-col>
        </b-row>
        <b-row class="diamondContainer">
          <b-col>
            <h3 class="fuenteDiamond">SOUND: “t”</h3>
          </b-col>
        </b-row>
      </b-col>
      <b-col sm="7">
        <tablaTC :cuestionario="tabla2P10" />
      </b-col>
    </b-row>
    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="3">
        <b-row>
          <b-col>
            <h3 class="subTitulo">Ending sounds</h3>
          </b-col>
        </b-row>
        <b-row class="diamondContainer">
          <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
          <b-col>
            <h3 class="fuenteDiamond">T, D.</h3>
          </b-col>
        </b-row>
        <b-row class="diamondContainer">
          <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
          <b-col>
            <h3 class="fuenteDiamond">
              The e sound at the end of a word is silent.
            </h3>
          </b-col>
        </b-row>
        <b-row class="diamondContainer">
          <b-col>
            <h3 class="fuenteDiamond">SOUND: “id”</h3>
          </b-col>
        </b-row>
      </b-col>
      <b-col sm="7">
        <tablaTC :cuestionario="tabla3P10" />
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
    inputChecked,
  },
  data() {
    return {
        tabla3P10: {
        fields: [
          { key: "a", label: "Present", thClass: "subTitulo" },
          { key: "b", label: "Past", thClass: "subTitulo" },
          { key: "c", label: "Pronunciación", thClass: "subTitulo" },
        ],
        items: [
          { a: "WANT", b: "WANTED", c: "<Wantid>" },
          { a: "DECIDE", b: "DECIDED", c: "<Disaidid>" },               
        ],
      },
        tabla2P10: {
        fields: [
          { key: "a", label: "Present", thClass: "subTitulo" },
          { key: "b", label: "Past", thClass: "subTitulo" },
          { key: "c", label: "Pronunciación", thClass: "subTitulo" },
        ],
        items: [
          { a: "WORK", b: "WORKED", c: "<Workt>" },
          { a: "FIX", b: "FIXED", c: "<Fixt>" },
          { a: "LAUGH", b: "LAUGHED", c: "<Laft>" },
          { a: "FINISH", b: "FINISHED", c: "<Finisht>" },
          { a: "MISS", b: "MISSED", c: "<Mist>" },
          { a: "STOP", b: "STOPED", c: "<Stoppt>" },          
        ],
      },
      tabla1P10: {
        fields: [
          { key: "a", label: "Present", thClass: "subTitulo" },
          { key: "b", label: "Past", thClass: "subTitulo" },
          { key: "c", label: "Pronunciación", thClass: "subTitulo" },
        ],
        items: [
          { a: "CLEAN", b: "CLEANED", c: "<Cliind>" },
          { a: "SMILE", b: "SMILED", c: "<Smaild>" },
          { a: "CLAIM", b: "CLAIMED", c: "<Cleimd>" },
          { a: "PLAY", b: "PLAYED", c: "<Pleid>" },
          { a: "POUR", b: "POURED", c: "<Poord>" },
          { a: "SUE", b: "SUED", c: "<Sud>" },
          { a: "LIVE", b: "LIVED", c: "<Livd>" },
          { a: "GRAB", b: "GRABED", c: "<Grabd>" },
          { a: "CLOG", b: "CLOGED", c: "<Clogd>" },
          { a: "CLOSE", b: "CLOSED", c: "<clouzd>" },
        ],
      },
      listadoCompletarP9: [
        {
          listado: ["tried"],
          textoA: "1.   The world health organization",
          textoD: "to stop the spread of the virus.",
          tamano: 53,
        },
        {
          listado: ["aplied"],
          textoA: "2.   I went to the embassy and",
          textoD: "for the visa.",
          tamano: 40,
        },
        {
          listado: ["cried"],
          textoA: "3.	We were so happy that we  ",
          textoD: "for joy.",
          tamano: 36,
        },
        {
          listado: ["dried"],
          textoA: "4.	The rays of sun ",
          textoD: "the wet grass.",
          tamano: 34,
        },
        {
          listado: ["copied"],
          textoA:
            "5.   The teacher didn’t give the student an A because he thinks the student",
          textoD: "and pasted the story.",
          tamano: 61,
        },
        {
          listado: ["replied"],
          textoA: "6.	He left his phone home however his wife",
          textoD: "all messages.",
          tamano: 51,
        },
        {
          listado: ["studied"],
          textoA: "7.	Nobody could believe I",
          textoD: "maths and physics at the university because ",
          textoD2:
            "I was too bad at solving mathematics operations at the school.",
          tamano: 60,
        },
      ],
      tablaCompleteP9: {
        fields: [
          { key: "a", thClass: "noHead" },
          { key: "b", thClass: "noHead" },
          { key: "c", thClass: "noHead" },
          { key: "d", thClass: "noHead" },
          { key: "e", thClass: "noHead" },
          { key: "f", thClass: "noHead" },
          { key: "g", thClass: "noHead" },
        ],
        items: [
          {
            a: "Study",
            b: "Apply",
            c: "Try",
            d: "Cry",
            e: "Reply",
            f: "Dry",
            g: "Copy",
          },
        ],
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
    };
  },
};
</script>

<style scoped>
/deep/ #tabla1P8 td {
  text-align: center !important;
}
</style>