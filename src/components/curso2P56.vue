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
        items: [{
            rojo:"1.The boy ",
            azul:"1. Is going to ",
            amarillo: "1. Do now "
        },
        {
            rojo:"2.Are you ",
            azul:"2. Was going to ",
            amarillo: "2. Be a great football player "
        },
        {
            rojo:"3.We ",
            azul:"3. Is supposed to ",
            amarillo: "3. Come here today "
        },
        {
            rojo:"4.Seth ",
            azul:"4. Was supposed to",
            amarillo: "4. Listen to music "
        },
        {
            rojo:"5. What is she ",
            azul:"5. Were going to ",
            amarillo: "5. Call her tomorrow "
        },
        {
            rojo:"6. I am ",
            azul:"6. Were supposed to ",
            amarillo: "6. Learn Spanish "
        },
        {
            rojo:"7. I",
            azul:"7. What are we ",
            amarillo: "7. Be fine "
        },
        {
            rojo:"",
            azul:"8. Going to ",
            amarillo: " "
        },
        {
            rojo:"",
            azul:"9. Supposed to ",
            amarillo: ""
        },
        {
            rojo:"",
            azul:"10. Are going to ",
            amarillo: ""
        }],
      },
    };
  },
};
</script>

<style>
</style>