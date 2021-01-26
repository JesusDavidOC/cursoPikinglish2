<template>
  <b-container fluid>
    <b-row>
      <b-col></b-col>
      <b-col sm="auto">
        <h3 class="titulo">MODIFIER SHALL</h3>
      </b-col>
      <b-col></b-col>
    </b-row>

    <b-row class="diamondContainer">
      <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
      <b-col>
        <h3 class="fuenteDiamond">
          Este auxiliar es igual que “Will” pero menos común y usualmente se usa
          con los sujetos “I y We”. además, se usa como auxiliar para pedir
          permiso.
        </h3>
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="auto">
        <h3 class="subTitulo">PEDIR CONSENTIMIENTO</h3>
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="auto">
        <tablaTC :cuestionario="tabla1P45" />
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="auto">
        <h3 class="subTitulo">ORACIONES EN FUTURO</h3>
      </b-col>
    </b-row>

    <b-col sm="1"></b-col>
    <b-col sm="auto">
      <p class="parrafo">Es igual que WILL, pero es menos común.</p>
    </b-col>

    <b-col sm="1"></b-col>
    <b-col sm="auto">
      <p class="parrafo">° I shall buy a new car (Compraré un nuevo carro) </p>
      <p class="parrafo">° We shall not go anywhere (No iremos a ningún lado) </p>
      <p class="parrafo">° Shall we go to New York? (¿Iremos a New York?) (¿Vamos a New York?)</p>
    </b-col>

    <b-row> </b-row>
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
      tabla1P45: {
        fields: [
          { key: "ESPAÑOL", label: "ESPAÑOL" },
          { key: "html1", label: "AUXILIAR" },
        ],
        items: [
          {
            ESPAÑOL: "¿Bailamos?",
            html1: "<span class='colorLetraRojo'>Shall</span> we dance?",
          },
          {
            ESPAÑOL: "¿me voy?",
            html1: "<span class='colorLetraRojo'>Shall</span> I go?",
          },
          {
            ESPAÑOL: "¿empezamos la clase?",
            html1:
              "<span class='colorLetraRojo'>Shall</span> we begin the class?",
          },
        ],
      },
    };
  },
};
</script>

<style>
</style>