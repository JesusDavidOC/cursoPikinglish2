<template>
  <b-container fluid>
    <b-row>
      <b-col></b-col>
      <b-col sm="auto">
        <h3 class="titulo">AM-IS-ARE + GOING TO + VERB.</h3>
      </b-col>
      <b-col></b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="10">
        <p class="parrafo">
          Esto se convierte en una fusión gramatical dando como resultado al
          español <strong>“Va a, voy a, vas a, vamos a y van a”</strong> más una
          acción.
        </p>
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="10">
        <tablaTC :cuestionario="tabla1P56" />
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="10">
        <p class="parrafo">Example:</p>
        <b-row>
          <b-col sm="1"></b-col>
          <b-col sm="auto">
            <p class="parrafo">
              ° It <span class="colorLetraRojo"> is going to </span>rain / Va a
              llover
            </p>
            <p class="parrafo">
              ° What <span class="colorLetraRojo">are </span> we
              <span class="colorLetraRojo">going to </span> do? / ¿Qué vamos a
              hacer?
            </p>
            <p class="parrafo">
              ° I <span class="colorLetraRojo">am not going to </span> travel /
              No voy a viajar
            </p>
          </b-col>
        </b-row>
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="auto">
        <h3 class="subTitulo">SINONIMOS DE IS, AM, ARE GOING TO</h3>
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="10">
        <p class="parrafo">
          En inglés también puede expresarse de la siguiente manera y tienen el
          mismo significado:
        </p>
      </b-col>
    </b-row>
    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="11">
        <p class="parrafo">1. en forma Progresiva</p>
        <b-row>
          <b-col sm="1"></b-col>
          <b-col sm="10">
            <p class="parrafo">
              <strong><i>I am working tomorrow until noon:</i></strong> esto
              puede significar “Yo estoy trabajando mañana hasta mediodía o yo
              voy a trabajar mañana hasta mediodía.
            </p>
          </b-col>
        </b-row>
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="11">
        <p class="parrafo">2. will be + progresivo (ing)</p>
        <b-row>
          <b-col sm="1"></b-col>
          <b-col sm="10">
            <p class="parrafo">
              <strong><i>I will be working tomorrow until noon:</i></strong>
              literalmente traduce “yo estaré trabajando mañana hasta mediodía”
              pero tiene el mismo significado de “I am going to work tomorrow”,
              es decir “yo voy a trabajar mañana”
            </p>
          </b-col>
        </b-row>
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="auto">
        <h3 class="subTitulo">
          EXERCICES: FILL IN THE GAPS WITH THE MISSING WORDS
        </h3>
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="11">
        <b-row
          v-for="(item, index) in listadoCompletarP57"
          :key="index + item.textoA"
          class="margin-bottom"
        >
          <b-col><inputCE :object="item" /></b-col>
        </b-row>
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
import inputCE from "./inputCEnriquecido";
import tablaTC from "./tablaTraduccionCodigos";
export default {
  components: {
    inputCE,
    tablaTC,
  },
  data() {
    return {
      listadoCompletarP57: [
        {
          lista1: ["am"],
          name: "inputCheked2",
          textoA: "1. Who are you going to visit? - I",
          textoD: "going to",
          tamano1: 36.8,
          lista2: ["visit"],
          textoD2: "my mum.(visit)",
          tamano2: 19.4,
        },
        {
          lista1: ["will"],
          name: "inputCheked2",
          textoA: "2. What will he be doing on vacation? - He",
          textoD: "be",
          tamano1: 40,
          lista2: ["surfing"],
          textoD2: "on his vacation. (surf)",
          tamano2: 25.5,
        },
        {
          lista1: ["is"],
          name: "inputCheked2",
          textoA: "3. Why is she going to Neiva? - She",
          textoD: "going Neiva to",
          tamano1: 42.4,
          lista2: ["sell"],
          textoD2: "some clothes. (sell)",
          tamano2: 22.4,
        },
        {
          lista1: ["am"],
          name: "inputCheked2",
          textoA: "4. When are you going to the gym? - I",
          textoD: "",
          tamano1: 35,
          lista2: ["going"],
          textoD2: "to the gym at 3pm. (go)",
          tamano2: 25.8,
        },
        {
          lista1: ["are"],
          name: "inputCheked2",
          textoA: "5. Who’s coming to the party? - Steven and John",
          textoD: "",
          tamano1: 42.4,
          lista2: ["coming"],
          textoD2: "to the party. (come)",
          tamano2: 24.4,
        },
        {
          lista1: ["am"],
          name: "inputCheked2",
          textoA: "6. Where are you going to stay tomorrow night? - I",
          textoD: "going to",
          tamano1: 48.5,
          lista2: ["stay"],
          textoD2: "in a hotel. (stay)",
          tamano2: 20.2,
        },
        {
          lista1: ["are"],
          name: "inputCheked2",
          textoA: "7. What are you going to do on your date tonight? - We",
          textoD: "going to",
          tamano1: 52,
          lista2: ["watch"],
          textoD2: "a film in the cinema. (watch)",
          tamano2: 29.8,
        },
        {
          lista1: ["will"],
          name: "inputCheked2",
          textoA: "8. What will you be doing this weekend? - Um, I don’t know, maybe I ",
          textoD: "be",
          tamano1: 57,
          lista2: ["playing"],
          textoD2: "tennis. (play)",
          tamano2: 20,
        },
        {
          lista1: ["am"],
          name: "inputCheked2",
          textoA: "9. Who are you going to see in the concert? - I",
          textoD: "going to",
          tamano1: 46,
          lista2: ["see"],
          textoD2: "Fall Out Boy! (see)",
          tamano2: 22,
        },
        {
          lista1: ["are"],
          name: "inputCheked2",
          textoA: "10. What are they going to do in town? - I think they",
          textoD: "going to",
          tamano1: 49.5,
          lista2: ["buy"],
          textoD2: "you a gift. (buy)",
          tamano2: 19.8,
        },
      ],
      tabla1P56: {
        fields: [
          { key: "col1", label: " ", thClass: "noHead" },
          { key: "html1", label: " ", thClass: "noHead" },
          { key: "col3", label: " ", thClass: "noHead" },
          { key: "col4", label: " ", thClass: "noHead" },
        ],
        items: [
          {
            col1: "AM",
            html1: "<span class='colorLetraRojo'>Going to</span>",
            col3: "Verb (Present)",
            col4: "Voy a…",
          },
          {
            col1: "IS",
            html1: "<span class='colorLetraRojo'>Going to</span>",
            col3: "Verb (Present)",
            col4: "Va a… ",
          },
          {
            col1: "ARE",
            html1: "<span class='colorLetraRojo'>Going to</span>",
            col3: "Verb (Present)",
            col4: "Vas a… vamos a… van a … ",
          },
        ],
      },
    };
  },
};
</script>

<style>
</style>