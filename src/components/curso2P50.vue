<template>
  <b-container fluid>
    <b-row>
      <b-col></b-col>
      <b-col sm="auto">
        <h3 class="titulo">OUGHT TO</h3>
      </b-col>
      <b-col></b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="auto">
        <p class="parrafo">
          <span class="colorLetraRojo">Negación:</span> OUGHT NOT
        </p>
        <p class="parrafo">
          <span class="colorLetraRojo">Significado:</span> Debería
        </p>
        <p class="parrafo"><span class="colorLetraRojo">Uso:</span></p>
        <p class="parrafo">
          1.Es igual que <span class="colorLetraRojo">SHOULD</span>, pero menos
          común.
        </p>
        <b-row>
          <b-col sm="1"></b-col>
          <b-col sm="auto">
            <p class="parrafo">
              Example:- We
              <span class="colorLetraRojo"> ought to </span>eat less
            </p>
          </b-col>
        </b-row>
        <p class="parrafo">
          2. Se usa para hablar de obligaciones y recomendaciones.
        </p>
        <b-row>
          <b-col sm="1"></b-col>
          <b-col sm="auto">
            <p class="parrafo">
              Example: - You
              <span class="colorLetraRojo"> ought to </span> finish your
              homework before you go out to play.
            </p>
          </b-col>
        </b-row>
        <p class="parrafo">
          3. No se usa con el sujeto “I” cuando se trata de un consejo y en
          lugar se usa “should”.
        </p>
        <b-row>
          <b-col sm="1"></b-col>
          <b-col sm="auto">
            <p class="parrafo">
              Example: - I
              <span class="colorLetraRojo">should</span> travel by bus rather
              than by plane
            </p>
          </b-col>
        </b-row>

        <p class="parrafo">
          4.Para hablar de una crítica o algo que no pasó en el pasado y
          lamentamos que no.
        </p>
        <b-row>
          <b-col sm="1"></b-col>
          <b-col sm="auto">
            <p class="parrafo">
              Example: -She
              <span class="colorLetraRojo"> ought to </span> have arrived in
              Moscow early this morning if the plane
            </p>

            <p class="parrafo">was on time.</p>
          </b-col>
        </b-row>
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="auto">
        <h3 class="subTitulo">
          PRACTICE. Fill up the gaps with Ought to or ought
        </h3>
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="11">
        <b-row
          v-for="(item, index) in listadoCompletarP50"
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
import inputChecked from "./inputChecked";
export default {
  components: {
    inputChecked,
  },
  data() {
    return {
      listadoCompletarP50: [
          {
          listado: ["should"],
          textoA: "1. Life is too short and time is precious therefore we",
          textoD: "live it intensively.",
          tamano: "58.5",
        },
        {
          listado: ["should"],
          textoA: "2. People ",
          textoD: "not drive a car without a license. They may be fined.",
          tamano: "53.8",
        },
        {
          listado: ["should"],
          textoA: "3. It is very dangerous to walk along the park late at night, parents ",
          textoD: "not  let their",
          textoD2:"children go out alone",
          tamano: "64",
        },
        {
          listado: ["should"],
          textoA: "4. You",
          textoD: " not speak with your mouth full.",
          tamano: "37.3",
        },
        {
          listado: ["should"],
          textoA: "5. Think about what I told you! I insist. You",
          textoD: "not call her anymore. ",
          tamano: "55",
        },
      ],
    };
  },
};
</script>

<style>
</style>