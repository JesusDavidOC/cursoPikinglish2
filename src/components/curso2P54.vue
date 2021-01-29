<template>
  <b-container fluid>
    <b-row>
      <b-col></b-col>
      <b-col sm="auto">
        <h3 class="titulo">WAS-WERE + SUPPOSED TO + VERB. </h3>
      </b-col>
      <b-col></b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="10">
        <p class="parrafo">
          Esta unión se convierte en una fusión gramatical dando como resultado al español “SE SUPONÍA QUE TENÍA QUE O DEBÍA”
        </p>
      </b-col>
    </b-row>

    

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="11">
        <tablaTC :cuestionario="tabla1P54" />
      </b-col>
    </b-row>

<b-row>
      <b-col sm="1"></b-col>
      <b-col sm="11">
        <p class="parrafo">Example:</p>
        <b-row>
          <b-col sm="1"></b-col>
          <b-col sm="auto">
            <p class="parrafo">
              ° I <span class="colorLetraRojo"> was supposed to</span>  do that  / Se suponía que yo tenía que hacer eso 
            </p>
            <p class="parrafo">
              ° What <span class="colorLetraRojo">was</span> i <span class="colorLetraRojo">supposed to</span> do then?    /    ¿Qué se suponía que tenía que hacer entonces? 
            </p>
            <p class="parrafo">
              ° You <span class="colorLetraRojo"> were not supposed to </span>  tell her that  /  No deberías decirle a ella eso 
            </p>
          </b-col>
        </b-row>
      </b-col>
    </b-row>
     <b-row>
      <b-col sm="auto">
        <h3 class="subTitulo">EXERCICES: Complete with was-were supposed to (negative as well) </h3>
      </b-col>
    </b-row>


    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="11">
        <b-row
          v-for="(item, index) in listadoCompletarP54"
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
    tablaTC,inputChecked
  },
  data() {
    return {
      tabla1P54: {
        fields: [
          { key: "col1", label: " ", thClass: "noHead" },
          { key: "html1", label: " ", thClass: "noHead" },
          { key: "col3", label: " ", thClass: "noHead" },
          { key: "col4", label: " ", thClass: "noHead" },
        ],
        items: [
          {
            col1: "WAS",
            html1: "<span class='colorLetraRojo'>Supposed to </span>",
            col3: "Verb (Present)",
            col4: "Se suponía que yo, él o ella tenía que…",
          },
          {
            col1: "WERE",
            html1: "<span class='colorLetraRojo'>Supposed to </span>",
            col3: "Verb (Present)",
            col4: "Se suponía que tú, nosotros o ellos tenías, teníamos o tenían que … ",
          },
        ],
      },

    listadoCompletarP54: [
          {
          listado: ["I'm not supposed to smoke here"],
          textoA: "1.(not smoke) This is a public building,",
          textoD: "",
          tamano: "53",
        },
        {
          listado: ["I'm not supposed to talk here"],
          textoA: "2.(not talk) This is a library,",
          textoD: "",
          tamano: "44",
        },
        {
          listado: ["He’s not supposed to be here"],
          textoA: "3.(not be here) John is on private land! ",
          textoD: "",
          tamano: "52",
        },
        {
          listado: ["You’re supposed to be doing your homework"],
          textoA: "4.(doing homework) Why are you on your phone?",
          textoD: "",
          tamano: "68",
        },
        {
          listado: ["you’re not supposed to steal"],
          textoA: "5.(not steal) I read the bible, God says",
          textoD: "",
          tamano: "51",
        },
        {
          listado: ["You’re supposed to use pesos"],
          textoA: "6.(use Pesos) This isn’t America, this is Colombia.",
          textoD: "",
          tamano: "60",
        },
        {
          listado: ["You’re supposed to drive on the road"],
          textoA: "7.(drive on the road) You can’t take your car on the grass!",
          textoD: "",
          tamano: "68.4",
        },
        {
          listado: ["he’s supposed to dress smartly"],
          textoA: "8.(dress smartly) He can’t wear that to an interview,",
          textoD: "",
          tamano: "61",
        },
        {
          listado: ["I’m supposed to bathe everyday"],
          textoA: "9.(bathe everyday) My mum says,",
          textoD: "",
          tamano: "50",
        },
        {
          listado: ["you’re not supposed to cheat"],
          textoA: "10.(not cheat) You copied during an official exam,",
          textoD: "",
          tamano: "59",
        },
        
      ],
    };
  },
};
</script>

<style>
</style>