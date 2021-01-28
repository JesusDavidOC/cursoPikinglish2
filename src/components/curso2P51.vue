<template>
  <b-container fluid>
    <b-row>
      <b-col></b-col>
      <b-col sm="auto">
        <h3 class="titulo">HAD BETTER</h3>
      </b-col>
      <b-col></b-col>
    </b-row>
    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="auto">
        <p class="parrafo">
          <span class="colorLetraRojo">Contracción y negación: </span>'d better,
          had better not
        </p>
        <p class="parrafo">
          <span class="colorLetraRojo">Significado:</span> Cuando creemos que
          algo es una buena idea de hacer algo.
        </p>
        <p class="parrafo">
          Es más usado en el inglés hablado y es igual que SHOULD.
        </p>
        <p class="parrafo"><span class="colorLetraRojo">Uso:</span></p>
        <b-row>
          <b-col sm="1"></b-col>
          <b-col sm="auto">
            <p class="parrafo">Example:</p>
            <b-row>
              <b-col sm="1"></b-col>
              <b-col sm="auto">
                <p class="parrafo">
                  ° You had better stop drinking. (Es mejor que dejes de tomar)
                </p>
                <p class="parrafo">
                  ° We had better take a taxi back home. (Es mejor que tomemos</p>
                 <p class="parrafo">   un taxi de regreso a casa)</p>
                 <p class="parrafo">
                  ° He had better save his money. (Él debería ahorrar su dinero) 
                </p>
                <p class="parrafo">
                  ° You had better tell the truth. (Es mejor si dices la verdad) 
                </p>
                <p class="parrafo">
                  ° It's raining, you had better not go out. (Está lloviendo, mejor no salgas)
                </p>
                <p class="parrafo">
                  ° You'd better not be late for work next time.</p> <p class="parrafo">(Más te vale que no llegues tarde al trabajo la próxima vez
                </p>
              </b-col>
            </b-row>
          </b-col>
        </b-row>
      </b-col>
    </b-row>


    <b-row>
      <b-col sm="auto">
        <h3 class="subTitulo">
          PRACTICE. Complete the gaps with had better or had better not 
        </h3>
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="11">
        <b-row
          v-for="(item, index) in listadoCompletarP51"
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
      listadoCompletarP51: [
          {
          listado: ["had better"],
          textoA: "1. If you keep drinking beer, you will get drunk so you",
          textoD: "go home now. ",
          tamano: "59.8",
        },
        {
          listado: ["had better"],
          textoA: "2. You",
          textoD: " write it down on a piece of paper.",
          tamano: "41.3",
        },
        {
          listado: ["had better"],
          textoA: "3. You are very sick! – you ",
          textoD: " not go to work today.",
          tamano: "46.3",
        },
        {
          listado: ["had better"],
          textoA: "4.  The party starts at 7:00 pm. You ",
          textoD: "be there in time to make sure everything is alright. ",
          tamano: "71",
        },
        {
          listado: ["had better"],
          textoA: "5.You",
          textoD: "stay home or you will get infected. ",
          tamano: "41.4",
        },
        {
          listado: ["had better"],
          textoA: "6. We",
          textoD: "hurry up or we will miss the bus. ",
          tamano: "40.3",
        },
        {
          listado: ["had better"],
          textoA: "7.  It is getting late and buses don’t run this time so I ",
          textoD: "go home now. ",
          tamano: "59",
        },
      ],
    };
  },
};
</script>

<style>
</style>