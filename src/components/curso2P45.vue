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
    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="auto">
        <p class="parrafo">Es igual que WILL, pero es menos común.</p>
      </b-col>
    </b-row>
    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="auto">
        <p class="parrafo">° I shall buy a new car (Compraré un nuevo carro)</p>
        <p class="parrafo"> ° We shall not go anywhere (No iremos a ningún lado)</p>
        <p class="parrafo">° Shall we go to New York? (¿Iremos a New York?) (¿Vamos a New York?)</p>
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="auto">
        <h3 class="subTitulo"> Let’s practice </h3>
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="11">
        <b-row
          v-for="(item, index) in listadoCompletarP45"
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
  </b-container>
</template>

<script>
import tablaTC from "./tablaTraduccionCodigos";
import inputChecked from "./inputChecked";
export default {
  components: {
    tablaTC,
    inputChecked,
  },
  data() {
    return {
      tabla1P45: {
        fields: [
          { key: "ESPAÑOL", label: "ESPAÑOL", thClass: "noHead"  },
          { key: "html1", label: "AUXILIAR", thClass: "noHead"  },
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

      listadoCompletarP45: [
        {
          listado: ["Shall"],
          textoA: "1. ",
          textoD: " we go? (<strong>¿Vamos?</strong>) ",
          tamano: 26,
        },
        {
          listado: ["Shall"],
          textoA: "2. ",
          textoD: "  we dance? (<strong>¿Bailamos?</strong>) ",
          tamano: 30.3,
        },
        {
          listado: ["Shall"],
          textoA: "3.I ",
          textoD: " travel to Europe  (<strong>Iré a Europa</strong>) ",
          tamano: 34.2,
        },
        {
          listado: ["Shall"],
          textoA: "4.I ",
          textoD: "  sit where I like  (<strong>Me sentaré donde me gusta</strong>) ",
          tamano: 44.2,
        },
        {
          listado: ["Shall"],
          textoA: "5.We",
          textoD: "see (<strong>Ya veremos</strong>) ",
          tamano: 27.5,
        },
        {
          listado: ["Shall"],
          textoA: "6. ",
          textoD: "we go now? (<strong>¿Nos vamos ahora?</strong>) ",
          tamano: 37,
        },
        {
          listado: ["Shall"],
          textoA: "7.I ",
          textoD: "  not fail (<strong>No voy a fallar</strong>) ",
          tamano: 29.6,
        },
        {
          listado: ["Shall"],
          textoA: "8. ",
          textoD: " we wait here? (<strong>¿Esperamos aqui?</strong>) ",
          tamano: 37.3,
        },
        {
          listado: ["Shall"],
          textoA: "9. ",
          textoD: " we revise what you’ve learnt? (<strong>¿Revisamos lo que has aprendido?</strong>) ",
          tamano: 59.7,
        },
        {
          listado: ["Shall"],
          textoA: "10.What ",
          textoD: "we watch? (<strong>¿Que vamos a ver?</strong>) ",
          tamano: 39.8,
        },
      ],
    };
  },
};
</script>

<style>
</style>