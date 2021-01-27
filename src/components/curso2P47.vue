<template>
  <b-container fluid>
    <b-row>
      <b-col></b-col>
      <b-col sm="auto">
        <h3 class="titulo">NEW SUPER POWER VERBS</h3>
      </b-col>
      <b-col></b-col>


    </b-row>
    <b-row>
    <b-col sm="1"></b-col>
    <b-col sm="auto">
      <p class="parrafo">
        Estos nuevos verbos denominados con poder son usados con el verbo en su
        forma presente, y tienen unas traducciones muy exactas al español, de
        modo que basta con leer sus funciones en diferentes contextos para crear
        oraciones interesantes en inglés.
      </p>
    </b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="auto">
        <tablaTC :cuestionario="tabla1P47" />
      </b-col>
    </b-row>

    <b-row class="diamondContainer">
      <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
      <p class="fuenteDiamond">
        Practiquemos los nuevos verbos con poder en contexto con ejemplos.
      </p>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="auto">
        <p class="parrafo">
          ° It hasn’t rained in ages. It
          <span class="colorLetraRojo"> might </span>rain this week / No ha
          llovido en mucho tiempo. Es posible que llueva esta semana.
        </p>
        <p class="parrafo">
          ° Stop saying she is crazy. she<span class="colorLetraRojo">
            may not </span
          >like it / Deja de decir que ella está loca. Puede que no le guste.
        </p>
        <p class="parrafo">
          ° If we want to pass the exam tomorrow we<span class="colorLetraRojo">
            study all night </span
          >like it / Si queremos pasar el examen mañana, deberíamos estudiar
          toda la noche.
        </p>
        <p class="parrafo">
          ° It is going to rain. You<span class="colorLetraRojo">
            ought to </span
          >take your umbrella or you will get wet / Va a llover. deberías llevar
          una sombrilla o te mojaras.
        </p>
        <p class="parrafo">
          ° I still<span class="colorLetraRojo"> have got </span>the present you
          gave me / Aún tengo el regalo que me diste.
        </p>
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
import tablaTC from "./tablaTraduccionCodigos";
export default {
  components: {
    tablaTC,
  },
  data() {
    return {
      tabla1P47: {
        fields: [
          { key: "html1", label: "1", thClass: "noHead" },
          { key: "col2", label: "2", thClass: "noHead" },
          { key: "col3", label: "3", thClass: "noHead" },
          { key: "col4", label: "4", thClass: "noHead" },
          { key: "col5", label: "5", thClass: "noHead" },
        ],
        items: [
          {
            html1: "<strong>MIGHT</strong>",
            col2: "Podría,es posible que,quizá,puede que",
            col3:
              "Para pedir permiso. (es más formal), para prohibiciones o cuando hay una probabilidad que depende de ti. Además, en casi todos los contextos es igual que el might",
            col4: "Present",
            col5: "Might not",
          },
          {
            html1: "<strong>MAY</strong>",
            col2: "Puede, puede que, es posible que",
            col3:
              "Cuando hay una probabilidad muy remota de que algo suceda o no. su forma pasada es might have + participio",
            col4: "Present",
            col5: "May not",
          },
          {
            html1: "<strong>OUGHT TO</strong>",
            col2: "Debería",
            col3:
              "Es muy poco usual, pero es importante saberlo y es usado para algo que está pasando en el momento y que tiene una consecuencia",
            col4: "Present",
            col5: "Ought not to",
          },
          {
            html1: "<strong>HAD BETTEAR</strong>",
            col2: "Más vale que, es mejor que no debería.",
            col3:
              "Se usa cuando aconsejamos porque hay una consecuencia negativa y puede sonar como una advertencia",
            col4: "Present",
            col5: "Had better not",
          },
          {
            html1: "<strong>HAVE GOT</strong>",
            col2: "Tener",
            col3:
              "Es lo mismo que HAVE, solo que este puede negarse y es más común en el inglés británico",
            col4: "Present",
            col5: "Haven't got",
          },
        ],
      },
    };
  },
};
</script>

<style>
</style>