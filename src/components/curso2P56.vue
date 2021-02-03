<template>
  <b-container>
    <b-row>
      <b-col></b-col>
      <b-col sm="auto">
        <h3 class="titulo">WAS-WERE + GOING TO + VERB</h3>
      </b-col>
      <b-col></b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="10">
        <p class="parrafo">
          Esto se convierte en una fusión gramatical dando como resultado al
          español “Iba a, Ibas a, Íbamos a, Iban a.
        </p>
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="10">
        <tablaTC :cuestionario="tabla1P58" />
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
              ° It <span class="colorLetraRojo"> was going to </span> be a sunny
              day but it rained. / Iba a ser un día soleado, pero llovió.
            </p>
            <p class="parrafo">
              ° I <span class="colorLetraRojo"> was not going </span> to say
              that / Yo no iba a decir eso.
            </p>
            <p class="parrafo">
              ° What <span class="colorLetraRojo">were </span>you
              <span class="colorLetraRojo"> going to </span> do? / ¿Qué ibas a
              hacer?
            </p>
            <p class="parrafo">
              ° They <span class="colorLetraRojo"> were going to </span> call
              you / Ellos iban a llamarte
            </p>
            <p class="parrafo">
              ° She <span class="colorLetraRojo"> was not going to </span> come
              / Ella no iba a venir.
            </p>
          </b-col>
        </b-row>
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="10">
        <tablaTC :cuestionario="tabla2P59" />
      </b-col>
    </b-row>


    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="11">
        <tablaTC :cuestionario="tabla3P59" />
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
      tabla1P58: {
        fields: [
          { key: "col1", label: " ", thClass: "noHead" },
          { key: "html1", label: " ", thClass: "noHead" },
          { key: "col3", label: " ", thClass: "noHead" },
          { key: "col4", label: " ", thClass: "noHead" },
        ],
        items: [
          {
            col1: "WAS",
            html1: "<span class='colorLetraRojo'>Going to</span>",
            col3: "Verb (Present)",
            col4: "Iba a…",
          },
          {
            col1: "WERE",
            html1: "<span class='colorLetraRojo'>Going to</span>",
            col3: "Verb (Present)",
            col4: "Ibas a… Ibamos a… Iban a… ",
          },
          {
            col1: "",
            html1: "",
            col3: "",
            col4:
              "Esta combinación puede traducirse como “Iba a, Ibas a, Íbamos a, Iban a.",
          },
        ],
      },
      tabla2P59: {
        fields: [
          { key: "rojo", label: " ", thClass: "Red" },
          { key: "azul", label: " ", thClass: "Blue" },
          { key: "amarillo", label: " ", thClass: "Yelow" },
        ],
        items: [
          {
            rojo: "1.The boy ",
            azul: "1. Is going to ",
            amarillo: "1. Do now ",
          },
          {
            rojo: "2.Are you ",
            azul: "2. Was going to ",
            amarillo: "2. Be a great football player ",
          },
          {
            rojo: "3.We ",
            azul: "3. Is supposed to ",
            amarillo: "3. Come here today ",
          },
          {
            rojo: "4.Seth ",
            azul: "4. Was supposed to",
            amarillo: "4. Listen to music ",
          },
          {
            rojo: "5. What is she ",
            azul: "5. Were going to ",
            amarillo: "5. Call her tomorrow ",
          },
          {
            rojo: "6. I am ",
            azul: "6. Were supposed to ",
            amarillo: "6. Learn Spanish ",
          },
          {
            rojo: "7. I",
            azul: "7. What are we ",
            amarillo: "7. Be fine ",
          },
          {
            rojo: "",
            azul: "8. Going to ",
            amarillo: " ",
          },
          {
            rojo: "",
            azul: "9. Supposed to ",
            amarillo: "",
          },
          {
            rojo: "",
            azul: "10. Are going to ",
            amarillo: "",
          },
        ],
      },
      tabla3P59: {
        fields: [
          { key: "rojo", label: " ", thClass: "Red" },
          { key: "amarillo", label: " ", thClass: "Blue" },
          { key: "azul", label: " ", thClass: "Yelow" },
          { key: "complejo1", label: "English", thClass: "" },
          { key: "español", label: "Spanish", thClass: "" },],
           items: [
          {
            rojo: "1",
            amarillo: "4",
            azul: "3",
            complejo1:  {
              lista: ["The boy was supposed to come here today"],
              tamano: 30.4,
              resultado: false,
            },
            español:"Se supone que el chico tenía que venir aquí hoy"
          },
          {
            rojo: "2",
            amarillo: "8",
            azul: "5",
            complejo1:  {
              lista: ["Are you going to call her tomorrow?"],
              tamano: 26,
              resultado: false,
            },
            español:"¿Vas a llamar la mañana?"
          },
          {
            rojo: "3",
            amarillo: "6",
            azul: "3",
            complejo1:  {
              lista: ["We were supposed to come here today"],
              tamano: 28,
              resultado: false,
            },
            español:"Nosotros debíamos venir aquí hoy"
          },
          {
            rojo: "4",
            amarillo: "1",
            azul: "2",
            complejo1:  {
              lista: ["Seth is going to be a great football player"],
              tamano: 29,
              resultado: false,
            },
            español:"Seth va a ser un gran jugador de futbol"
          },
           {
            rojo: "5",
            amarillo: "8",
            azul: "1",
            complejo1:  {
              lista: ["What is she going to do now?"],
              tamano: 22.8,
              resultado: false,
            },
            español:"¿Qué va ella a hacer ahora?"
          },
          {
            rojo: "6",
            amarillo: "8",
            azul: "7",
            complejo1:  {
              lista: ["I am going to be fine"],
              tamano: 17.4,
              resultado: false,
            },
            español:"Yo voy a estar bien"
          },
          {
            rojo: "6",
            amarillo: "9",
            azul: "6",
            complejo1:  {
              lista: ["I am supposed to learn Spanish"],
              tamano: 24,
              resultado: false,
            },
            español:"Yo debo aprender español"
          },
          {
            rojo: "3",
            amarillo: "10",
            azul: "4",
            complejo1:  {
              lista: ["We are going to listen to music"],
              tamano: 23.4,
              resultado: false,
            },
            español:"Nosotros vamos a escuchar música"
          },
          {
            rojo: "1",
            amarillo: "1",
            azul: "4",
            complejo1:  {
              lista: ["The boy is going to listen to music"],
              tamano: 25,
              resultado: false,
            },
            español:"El chico va a escuchar música"
          },
          {
            rojo: "4",
            amarillo: "2",
            azul: "2",
            complejo1:  {
              lista: ["Seth was going to be a great football player"],
              tamano: 30.8,
              resultado: false,
            },
            español:"Seth iba a ser un gran jugador de futbol"
          },
           {
            rojo: "5",
            amarillo: "9",
            azul: "1",
            complejo1:  {
              lista: ["What is she supposed to do now?"],
              tamano: 25,
              resultado: false,
            },
            español:"¿Qué se supone que ella debe hacer?"
          },
           {
            rojo: "4",
            amarillo: "4",
            azul: "5",
            complejo1:  {
              lista: ["Seth was supposed to call her tomorrow"],
              tamano: 29,
              resultado: false,
            },
            español:"Seth debía llamarla a ella mañana"
          },
          {
            rojo: "1",
            amarillo: "1",
            azul: "2",
            complejo1:  {
              lista: ["The boy is going to be a great football player"],
              tamano: 31.4,
              resultado: false,
            },
            español:"El chico va a hacer un gran jugador de futbol"
          },
          {
            rojo: "2",
            amarillo: "8",
            azul: "6",
            complejo1:  {
              lista: ["Are you going to learn Spanish?"],
              tamano: 24,
              resultado: false,
            },
            español:"¿Vas a aprender español?"
          },
          {
            rojo: "7",
            amarillo: "4",
            azul: "5",
            complejo1:  {
              lista: ["I was supposed to call her tomorrow"],
              tamano: 26.4,
              resultado: false,
            },
            español:"Yo debí llamarla a ella mañana"
          },
          {
            rojo: "6",
            amarillo: "8",
            azul: "7",
            complejo1:  {
              lista: ["I am going to be fine"],
              tamano: 17.4,
              resultado: false,
            },
            español:"Yo voy a estar bien"
          },
          {
            rojo: "3",
            amarillo: "5",
            azul: "4",
            complejo1:  {
              lista: ["We were going to listen to music"],
              tamano: 24,
              resultado: false,
            },
            español:"Nosotros íbamos a escuchar música"
          },
        ],
      },
    };
  },
};
</script>

<style>
</style>