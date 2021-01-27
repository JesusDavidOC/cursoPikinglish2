<template>
  <b-container fluid>
    <b-row>
      <b-col></b-col>
      <b-col sm="auto">
        <h3 class="titulo">MODIFIER WILL</h3>
      </b-col>
      <b-col></b-col>
    </b-row>

    <b-row class="diamondContainer">
      <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
      <p class="fuenteDiamond">Este es el auxiliar del futuro.</p>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
        <b-col sm="auto">
          <p class="parrafo"><strong><br />-También se usa para pedir un favor muy formal y tiene un significado similar a Podría o quiere usted.</strong></p>
        <p class="parrafo">° Will you sit down, please? (¿Podría usted sentarse, por favor? O ¿Quiere usted sentarse por favor?.</p>
        <p class="parrafo">° Will you close the door, please?</p>
        <p class="parrafo">° Will you help me carry these bags?</p>

        <p class="parrafo">
          <strong
            ><br />- También significa SOLER, es decir tener el hábito
            de.</strong
          >
        </p>
        <p class="parrafo">
          ° He will always tell you about his experiences in the army even if
          you are not interested in it.
        </p>
        <p class="parrafo">° I will sit on a chair thinking about my plans</p>
        <p class="parrafo">° She will talk about her trips for hours on en</p>

        <p class="parrafo">
          <strong
            ><br />- Además, significa testamento, voluntad o albedrío.</strong
          >
        </p>
        <p class="parrafo">
          ° Her father left her the house in his will. (Su padre le dejó la casa
          en su testamento)
        </p>
        <p class="parrafo">° Force of Will: fuerza de voluntad</p>
        <p class="parrafo">° Free will: libre albedrío</p>
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="auto">
        <h3 class="subTitulo">COMPLETA CON WILL O SHALL</h3>
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="11">
        <b-row
          v-for="(item, index) in listadoCompletarP46"
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
    inputChecked,
  },
  data() {
    return {
      listadoCompletarP46: [
        {
          listado: ["Shall"],
          textoA: "1.",
          textoD: "we have breakfast? ",
          tamano: 26.1,
        },
        {
          listado: ["Will"],
          textoA: "2. Are you sure it",
          textoD: "be easy?",
          tamano: 28.4,
        },
        {
          listado: ["Will"],
          textoA: "3.",
          textoD: " she have sugar in her tea?",
          tamano: 30.2,
        },
        {
          listado: ["Will"],
          textoA: "4. Do you think Victor ",
          textoD: "help me?",
          tamano: 31.5,
        },
        {
          listado: ["Will"],
          textoA: "5. How long ",
          textoD: "they stay for?",
          tamano: 28,
        },
        {
          listado: ["Will"],
          textoA: "6. I hope we ",
          textoD: "be home by 10",
          tamano: 29.3,
        },
        {
          listado: ["Shall"],
          textoA: "7.",
          textoD: "I wait for you? ",
          tamano: 22.4,
        },
        {
          listado: ["Will"],
          textoA: "8. I",
          textoD: "we have breakfasbe 18 next yeart?",
          tamano: 36.5,
        },
        {
          listado: ["Shall"],
          textoA: "9. What",
          textoD: "I cook tonight ",
          tamano: 26,
        },
        {
          listado: ["Will"],
          textoA: "10. I’ve finished the exercise, what",
          textoD: "I do now",
          tamano: 39.8,
        },
      ],
    };
  },
};
</script>

<style>
</style>