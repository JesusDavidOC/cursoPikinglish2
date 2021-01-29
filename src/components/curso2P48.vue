<template>
  <b-container fluid>
    <b-row>
      <b-col></b-col>
      <b-col sm="auto">
        <h3 class="titulo">MIGHT</h3>
      </b-col>
      <b-col></b-col>
    </b-row>
    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="auto">
        <p class="parrafo">
          <span class="colorLetraRojo">Negación:</span> MIGHT NOT
        </p>
        <p class="parrafo">
          <span class="colorLetraRojo">Significado:</span> Es posible que,
          podría, puede que y solía.
        </p>
        <p class="parrafo"><span class="colorLetraRojo">Uso:</span></p>
        <p class="parrafo">
          1.Cuando existe la posibilidad y preferimos hacer algo en el futuro.
        </p>
        <b-row>
          <b-col sm="1"></b-col>
          <b-col sm="auto">
            <p class="parrafo">
              Example: There are black clouds in the sky, it
              <span class="colorLetraRojo">might</span> rain later
            </p>
          </b-col>
        </b-row>
        <p class="parrafo">
          2. Se usa en el pasado cuando se refiere a algo repetitivo como una
          norma o hábito.
        </p>
        <b-row>
          <b-col sm="1"></b-col>
          <b-col sm="auto">
            <p class="parrafo">
              Example: In 1984 American children
              <span class="colorLetraRojo">might</span> go to school in uniform.
            </p>
          </b-col>
        </b-row>
        <p class="parrafo">
          3. Algo que podría haber sido o pasado o para criticar algo que debió
          haberse
        </p>
        <p class="parrafo">
          hecho como creemos y la estructura es: MIGHT + HAVE + PARTICIPLE
        </p>
        <b-row>
          <b-col sm="1"></b-col>
          <b-col sm="auto">
            <p class="parrafo">
              Example: She
              <span class="colorLetraRojo">might have</span> waited
            </p>
          </b-col>
        </b-row>
      </b-col>
    </b-row>

   <b-row>
      <b-col sm="auto">
        <h3 class="subTitulo">PRACTICE. Fill out the gaps with MIGHT.</h3>
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="11">
        <b-row
          v-for="(item, index) in listadoCompletarP48"
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
          />
          </b-col>
        </b-row>
        <b-col> <inputCE :object="listadoCompletar2P48"/></b-col>
      </b-col>
    </b-row>


  </b-container>
</template>

<script>
import inputChecked from "./inputChecked";
import inputCE from "./inputCEnriquecido";
export default {
  components: {
    inputChecked,inputCE,
  },
  data() {
    return {
      listadoCompletarP48: [
        {
          listado: ["might"],
          textoA: "1. She is busy now but she ",
          textoD: " come later.",
          tamano: 37.5,
        },
        {
          listado: ["might"],
          textoA: "2. If you litter on the street, you ",
          textoD: "get fined by the authorities.",
          tamano: 50.9,
        },
        {
          listado: ["might"],
          textoA: "3. There are a lot of robbers in the city Centre. -Watch out! You",
          textoD: " be robbed",
          tamano: 60.8,
        },
        {
          listado: ["might"],
          textoA: "4. You should take an umbrella, it",
          textoD: "rain later.",
          tamano: 40.8,
        },
        {
          listado: ["might"],
          textoA: "5.  I thought you",
          textoD: " have come.",
          tamano: 30.4,
        },
        {
          listado: ["might"],
          textoA: "6. She decided not to come but I think she ",
          textoD: "I wait for you? ",
          tamano: 49.6,
        },
        {
          listado: ["might"],
          textoA: "7. I",
          textoD: "paint the kitchen blue next week.",
          tamano: 36.4,
        },
        {
          listado: ["might"],
          textoA: "8. If you burn the dried leaves you",
          textoD: "cause a fire.",
          tamano: 43,
        },
        {
          listado: ["might"],
          textoA: "9. aqui va un input cheket enriqucido",
          textoD: "I do now",
          tamano: 39.8,
        },
      ],
      listadoCompletar2P48:{
            lista1:["might"],
            name:"inputCheked1",
            textoA:"10. We",
            textoD:"go swimming in the river or we",
            tamano1:36.2,
            lista2:["might"],
            textoD2:"not",
            tamano2:12.4,
        }
    };
  },
};
</script>

<style>
</style>