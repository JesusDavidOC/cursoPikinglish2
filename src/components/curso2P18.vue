<template>
  <b-container fluid>
    <b-row>
      <b-col></b-col>
      <b-col sm="auto">
        <h3 class="titulo">THE USE OF THE AUXILIARIES</h3>
      </b-col>
      <b-col></b-col>
    </b-row>
    <b-row>
      <b-col></b-col>
      <b-col sm="8">
        <p class="parrafo">
          The five (5) auxiliaries are words that don’t have any translation and
          they are simply used to ask questions and negate sentences.
        </p>
      </b-col>
      <b-col></b-col>
    </b-row>
    <b-row v-for="item in tablasP18" :key="item">
      <b-col></b-col>
      <b-col>
        <img :src="item" alt="tablasP18" />
      </b-col>
      <b-col></b-col>
    </b-row>
    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="auto">
        <b-row
          v-for="(item, index) in listadoInputsP19"
          :key="'listadoInputsP19' + index"
        >
          <b-row>
            <h4>
              <strong>{{ item.pregunta }}</strong>
            </h4>
          </b-row>
          <b-row> </b-row>
          <inputChecked
            :esperado="item.esperado"
            :tamano="item.tamano"
            :conTexto="true"
            :textoA="item.textoA"
            :textoD="item.textoD"
            :textoD2="item.textoD2"
          />
        </b-row>
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
import opcionMultiple from "./opcionMultiple";
import inputChecked from "./inputChecked";
import tablaTC from "./tablaTraduccionCodigos";
import audioComp from "./audioComp";
export default {
  components: {
    inputChecked,
  },
  data() {
    return {
      tablasP18: [
        "https://classroom.pikinglish.com/cursos/curso2/leccion4/img/tabla1P18.PNG",
        "https://classroom.pikinglish.com/cursos/curso2/leccion4/img/tabla2P18.PNG",
        "https://classroom.pikinglish.com/cursos/curso2/leccion4/img/tabla3P18.PNG",
        "https://classroom.pikinglish.com/cursos/curso2/leccion4/img/tabla4P18.PNG",
        "https://classroom.pikinglish.com/cursos/curso2/leccion4/img/tabla5P18.PNG",
      ],
      listadoInputsP19: [
        {
          esperado: ["Bought"],
          presgunta: "1.	What did you buy?",
          textoA: "I",
          textoD: "a pair of shoes",
          tamano: 19.8,
        },
        {
          esperado: ["went"],
          pregunta: "2.	Where did you go?",
          textoA: "I",
          textoD: "nowhere",
          tamano: 14.5,
        },
        {
          esperado: ["spoke"],
          pregunta: "3.	Who did you speak to?",
          textoA: "I",
          textoD: "to Michael",
          tamano: 16.4,
        },
        {
          esperado: ["felt"],
          pregunta: "4.	How did you feel?",
          textoA: "I",
          textoD: "very good",
          tamano: 14.5,
        },
        {
          esperado: ["met"],
          pregunta: "5.	When did you meet Victor?",
          textoA: "I",
          textoD: "him a couple weeks ago",
          tamano: 24.3,
        },
        {
          esperado: ["drank"],
          pregunta: "6.	How many  glasses of milk did you drink?",
          textoA: "I",
          textoD: "six of them.",
          tamano: 17,
        },
        {
          esperado: ["saw"],
          pregunta: "7.	What time did you see Britney?",
          textoA: "I",
          textoD: "her at about 6:00 am",
          tamano: 22,
        },
        {
          esperado: ["taught"],
          pregunta: "8.	What did you teach students?",
          textoA: "I",
          textoD: "them how to deal with a breakup .",
          tamano: 32,
        },
        {
          esperado: ["took"],
          pregunta: "9.	Where did you take your children yesterday?",
          textoA: "I",
          textoD: "them to the swimming pool.",
          tamano: 26.7,
        },
        {
          esperado: ["found"],
          pregunta: "10.	What did you find?",
          textoA: "I",
          textoD: "a ring",
          tamano: 13,
        },
        {
          esperado: ["wore"],
          pregunta: "11.	What did you wear to the party last night?",
          textoA: "I",
          textoD: "a beautiful red dress.",
          tamano: 22.8,
        },
        {
          esperado: ["ran"],
          pregunta: "12.	I saw you running yesterday, how far did you run?",
          textoA: "I",
          textoD: "nearly 10 km.",
          tamano: 16.8,
        },
        {
          esperado: ["flew"],
          pregunta: "13.	Welcome to Colombia! Where did you fly in from?",
          textoA: "I",
          textoD: "in from London. It was a long journey!",
          tamano: 33.3,
        },
        {
          esperado: ["threw"],
          pregunta: "14.	Did you throw that stone at me?",
          textoA: "No, Johnny",
          textoD: "it at you.",
          tamano: 22,
        },
        {
          esperado: ["left"],
          pregunta: "15.	What time did you leave the party last night?",
          textoA: "I",
          textoD: "at 11pm, I think. I was so tired.",
          tamano: 28,
        },
      ],
    };
  },
};
</script>

<style>
</style>