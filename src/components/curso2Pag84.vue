<template>
  <div>
    <b-container fluid>
      <b-row>
        <b-col></b-col>
        <b-col sm="auto">
          <h3 class="titulo">INFORMATION QUESTIONS</h3>
        </b-col>
        <b-col></b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            Observa el cuadro y analiza la posición de las palabras para hacer
            preguntas de información.
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="10">
          <tablaTC :cuestionario="tabla3P7" />
        </b-col>
      </b-row>

      <br />
      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            <b>EXCEPTION: </b>Cuando preguntes por “quién o quiénes” hacen o
            hicieron algo en presente o pasado no se necesita auxiliar DO,DOES
            ni DID. solo basta con usar Who más el verbo en su forma presente o
            pasado. Pero si la pregunta lleva un sujeto si va auxiliar
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="11">
          <h3 class="subTitulo">
            PREGUNTAS CON WHO Y SIN SUJETO. (NO AUXILIAR)
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            <b>-</b> Who has a pen? ¿Quién tiene un lapicero?
          </h3>
        </b-col>
      </b-row>

      <br />
      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            <b>-</b> Who lives in this house? ¿Quién vive en esta casa?
          </h3>
        </b-col>
      </b-row>

      <br />
      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            <b>-</b> Who bought this cookie? ¿Quién compró esta galleta?
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="11">
          <h3 class="subTitulo">
            PREGUNTAS CON WHO Y CON SUJETO. (SI AUXILIAR)
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC"><b>-</b> Who do you love? ¿A quién amas?</h3>
        </b-col>
      </b-row>

      <br />
      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            <b>-</b> Who do you live with? ¿Con quién vives?
          </h3>
        </b-col>
      </b-row>

      <br />
      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            <b>-</b> Who did you talk to? ¿Con quién hablaste?
          </h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            Elige la respuesta correcta en las siguientes preguntas.
          </h3>
        </b-col>
      </b-row>

      <br />
      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC"><b>1. </b> Who</h3>
        </b-col>
        <b-col sm="left">
          <inputChecked :resuelto="false" :esperado="['saw']" tamano="10" />
        </b-col>
        <b-col sm="4">
          <h3 class="parrafoIC">Victor? (¿Quién vio a Victor?)</h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC"><b>a.</b>Did you see</h3>
        </b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC"><b>b.</b>sees</h3>
        </b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC"><b>c.</b>saw</h3>
        </b-col>
      </b-row>

      <br />
      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC"><b>2. </b> Who</h3>
        </b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['you work']"
            tamano="13"
          />
        </b-col>
        <b-col sm="4">
          <h3 class="parrafoIC">for? (¿Para quién trabajas?)</h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC"><b>a.</b>Works you</h3>
        </b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC"><b>b.</b>do you work</h3>
        </b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC"><b>c.</b>you work</h3>
        </b-col>
      </b-row>

      <br />
      <b-row>
        <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            Complete the questions according to the answer given.
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="10">
          <tablaTC :cuestionario="tabla2P7" />
        </b-col>
      </b-row>

      <br /><br />
      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="6">
          <tablaTC :cuestionario="tabla4P7" />
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="6">
          <tablaTC :cuestionario="tabla5P7" />
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
import posiblesRespuestasTabla from "./posiblesRespuestasTabla";
import opcionMultiple from "./opcionMultiple";
import listaIndex from "./listaIndex";
import inputChecked from "./inputChecked";
import tablaTC from "./tablaTraduccionCodigos";
import inputCheckedE from "./inputCEnriquecido";
import InputChecked from "./inputChecked.vue";
export default {
  components: {
    tablaTC,
    inputChecked,
    listaIndex,
    opcionMultiple,
    posiblesRespuestasTabla,
    inputCheckedE,
  },
  data() {
    return {
      tabla2P7: {
        fields: [
          { key: "a", label: "" },
          { key: "complejo1", label: "QUESTION" },
          { key: "c", label: "" },
        ],
        items: [
          {
            a: "The mouse ate a slice of cheese.",
            complejo1: {
              lista: ["What did the mouse eat?"],
              tamano: 23,
              resuelto: false,
            },
            c: "A slice of cheese",
          },
          {
            a: "Seth could escape from the shark",
            complejo1: { lista: ["could scape from the shark"], textoA:"Who", textoD:"?", tamano: 23, resuelto: false },
            c: "Seth",
          },
          {
            a: "They have bought a car",
            complejo1: { lista: ["have they bought"],textoA:"What",textoD:"?", tamano: 23, resuelto: false },
            c: "A car",
          },
          {
            a: "I seldom go to the movies",
            complejo1: { lista: ["do you go to the movies"],textoA:"How often",textoD:"?", tamano: 23, resuelto: false },
            c: "Seldom",
          },
          {
            a: "I have a cold because I got wet ",
            complejo1: { lista: ["do you have a cold"],textoA:"Why",textoD:"?", tamano: 23, resuelto: false },
            c: "Because I got wet",
          },
          {
            a: "We are looking for an apartment",
            complejo1: { lista: ["are they lookong for"], textoA:"What",texotD:"?", tamano: 23, resuelto: false },
            c: "An apartment",
          },
          {
            a: "I like the red one",
            complejo1: { lista: ["do you like"],textoA:"Which one",textoD:"?", tamano: 23, resuelto: false },
            c: "The red one",
          },
          {
            a: "I live up in the mountain",
            complejo1: { lista: ["do you live"],textoA:"Where",textoD:"?", tamano: 23, resuelto: false },
            c: "Up in the mountain",
          },
          {
            a: "I was talking to her",
            complejo1: { lista: ["was talking to her"],textoA:"Who",textoD:"?", tamano: 23, resuelto: false },
            c: "I",
          },
          {
            a: "She has two brothers",
            complejo1: { lista: ["brothers does she have"], textoA:"How many", textoD:"?", tamano: 23, resuelto: false },
            c: "Two",
          },
          {
            a: "I am 33 years old",
            complejo1: { lista: ["are you"], textoA:"How old", textoD:"?", tamano: 23, resuelto: false },
            c: "33",
          },
          {
            a: "My mother ́s name is Michelle",
            complejo1: { lista: ["is your mother´s name"], textoA:"What", textoD:"?", tamano: 23, resuelto: false },
            c: "Michelle",
          },
          {
            a: "They were there at 10:00 pm",
            complejo1: { lista: ["were there at 10:00 pm"], textoA:"Who", textoD:"?", tamano: 23, resuelto: false },
            c: "They",
          },
          {
            a: "They were at the school at 10:00",
            complejo1: { lista: ["time were they at school"], textoA:"What", textoD:"?", tamano: 23, resuelto: false },
            c: "10:00",
          },
          {
            a: "I am going to the supermarket",
            complejo1: { lista: ["are you going"], textoA:"Where", textoD:"?", tamano: 23, resuelto: false },
            c: "To the supermarket",
          },
          {
            a: "This one costs $100 dollar",
            complejo1: { lista: ["does that one cost"], textoA:"How much", textoD:"?", tamano: 23, resuelto: false },
            c: "$ 100 dollar",
          },
          {
            a: "I'd like to eat a sandwich",
            complejo1: { lista: ["would you like to eat"], textoA:"What", textoD:"?", tamano: 23, resuelto: false },
            c: "A sandwich",
          },
          {
            a: "She was born in 1984",
            complejo1: { lista: ["was she born"], textoA:"When", textoD:"?", tamano: 23, resuelto: false },
            c: "In 1984",
          },
          {
            a: "I have been sick",
            complejo1: { lista: ["have you been"], textoA:"How", textoD:"?", tamano: 23, resuelto: false },
            c: "Sick",
          },
        ],
      },
      tabla5P7: {
        fields: [
          { key: "a", label: "", thClass: "Yelow" },
          { key: "b", label: "", thClass: "Green" },
          { key: "c", label: "", thClass: "Blue" },
          { key: "d", label: "", thClass: "Red" },
          { key: "complejo1", label: "Informacion questions" },
        ],
        items: [
          {
            a: "1",
            b: "1",
            c: "1",
            d: "1",
            complejo1: {
              lista: ["How do you feel today"],
              tamano: 21.5,
              resuelto: false,
            },
          },
          {
            a: "2",
            b: "3",
            c: "7",
            d: "2",
            complejo1: {
              lista: ["Why did you do that"],
              tamano: 20,
              resuelto: false,
            },
          },
          {
            a: "3",
            b: "5",
            c: "8",
            d: "4",
            complejo1: {
              lista: ["Who were you talking to"],
              tamano: 22.5,
              resuelto: false,
            },
          },
          {
            a: "4",
            b: "8",
            c: "7",
            d: "2",
            complejo1: {
              lista: ["When can i do that"],
              tamano: 19.5,
              resuelto: false,
            },
          },
          {
            a: "5",
            b: "3",
            c: "7",
            d: "1",
            complejo1: {
              lista: ["What did you do today"],
              tamano: 22,
              resuelto: false,
            },
          },
          {
            a: "5",
            b: "5",
            c: "4",
            d: "5",
            complejo1: {
              lista: ["What were you doing in the car"],
              tamano: 26.5,
              resuelto: false,
            },
          },
          {
            a: "7",
            b: "7",
            c: "5",
            d: "7",
            complejo1: {
              lista: ["What time are you coming tomorrow"],
              tamano: 29.5,
              resuelto: false,
            },
          },
          {
            a: "8",
            b: "4",
            c: "3",
            d: "2",
            complejo1: {
              lista: ["How long have you been doing that"],
              tamano: 29,
              resuelto: false,
            },
          },
          {
            a: "1",
            b: "4",
            c: "3",
            d: "2",
            complejo1: {
              lista: ["How have you been doing that"],
              tamano: 26,
              resuelto: false,
            },
          },
          {
            a: "5",
            b: "4",
            c: "3",
            d: "6",
            complejo1: {
              lista: ["What have you been doing lately"],
              tamano: 27.5,
              resuelto: false,
            },
          },
          {
            a: "5",
            b: "8",
            c: "7",
            d: "X",
            complejo1: {
              lista: ["What can i do"],
              tamano: 17,
              resuelto: false,
            },
          },
          {
            a: "1",
            b: "8",
            c: "6",
            d: "X",
            complejo1: {
              lista: ["How can i help you"],
              tamano: 20,
              resuelto: false,
            },
          },
          {
            a: "7",
            b: "3",
            c: "2",
            d: "8",
            complejo1: {
              lista: ["What time did you arrive at the school"],
              tamano: 30.5,
              resuelto: false,
            },
          },
          {
            a: "5",
            b: "7",
            c: "8",
            d: "3",
            complejo1: {
              lista: ["What are you talking about"],
              tamano: 25,
              resuelto: false,
            },
          },
          {
            a: "5",
            b: "5",
            c: "4",
            d: "5",
            complejo1: {
              lista: ["What were you doing in the car"],
              tamano: 27,
              resuelto: false,
            },
          },
          {
            a: "5",
            b: "6",
            c: "4",
            d: "1",
            complejo1: {
              lista: ["What is she doing today"],
              tamano: 23,
              resuelto: false,
            },
          },
          {
            a: "6",
            b: "3",
            c: "7",
            d: "2",
            complejo1: {
              lista: ["Where did you do that"],
              tamano: 22,
              resuelto: false,
            },
          },
          {
            a: "2",
            b: "4",
            c: "3",
            d: "2",
            complejo1: {
              lista: ["Why have you been doing that"],
              tamano: 26,
              resuelto: false,
            },
          },
          {
            a: "7",
            b: "1",
            c: "2",
            d: "8",
            complejo1: {
              lista: ["What time do you arrive at the school"],
              tamano: 30,
              resuelto: false,
            },
          },
          {
            a: "3",
            b: "5",
            c: "8",
            d: "4",
            complejo1: {
              lista: ["Who were you talking to"],
              tamano: 23,
              resuelto: false,
            },
          },
          {
            a: "1",
            b: "6",
            c: "X",
            d: "1",
            complejo1: {
              lista: ["How is she today"],
              tamano: 20,
              resuelto: false,
            },
          },
          {
            a: "1",
            b: "7",
            c: "X",
            d: "1",
            complejo1: {
              lista: ["How are you today"],
              tamano: 20,
              resuelto: false,
            },
          },
        ],
      },
      tabla4P7: {
        fields: [
          { key: "a", label: "", thClass: "Yelow" },
          { key: "b", label: "", thClass: "Green" },
          { key: "c", label: "", thClass: "Blue" },
          { key: "d", label: "", thClass: "Red" },
        ],
        items: [
          {
            a: "1. How",
            b: "1. Do you",
            c: "1. Feel",
            d: "1. today",
          },
          {
            a: "2. Why",
            b: "2. Does she",
            c: "2. Arrive at",
            d: "2. That",
          },
          {
            a: "3. Who",
            b: "3. Did you",
            c: "3. Been doing",
            d: "3. About",
          },
          {
            a: "4. When",
            b: "4. Have you",
            c: "4. Doing",
            d: "4. To",
          },
          {
            a: "5. What",
            b: "5. Were you",
            c: "5. Coming",
            d: "5.  In the car",
          },
          {
            a: "6. Where",
            b: "6. Is she",
            c: "6. Help you",
            d: "6. Lately",
          },
          {
            a: "7. What time",
            b: "7. Are you",
            c: "7. Do",
            d: "7. Tomorrow",
          },
          {
            a: "8. How long",
            b: "8. Can i",
            c: "8. Talking",
            d: "8. The school",
          },
        ],
      },
      tabla3P7: {
        fields: [
          { key: "a", label: "Question" },
          { key: "b", label: "W/Question" },
          { key: "c", label: "Verb" },
          { key: "d", label: "Answer" },
        ],
        items: [
          {
            a: "¿Qué quieres decir?",
            b: "What",
            c: "Do",
            d: "mean?",
          },
          {
            a: "¿Dónde se lleva a cabo el juego cada año?",
            b: "Where",
            c: "Does",
            d: "The game take place every year?",
          },
          {
            a: "¿Por qué hiciste eso?",
            b: "Why",
            c: "Did",
            d: "You do that?",
          },
          {
            a: "¿Cómo le gustaría hacer eso?",
            b: "How",
            c: "Would",
            d: "You like to do that?",
          },
          {
            a: "¿Cuánto tiempo te quedarás en USA?",
            b: "How long",
            c: "Will",
            d: "You stay here in the United States?",
          },
          {
            a: "¿Cuándo es tú cumpleaños?",
            b: "When",
            c: "Is",
            d: "Your birthday?",
          },
          {
            a: "¿Con quién estás?",
            b: "Who",
            c: "Are",
            d: "you with?",
          },
          {
            a: "¿Qué estoy hacienda aquí?",
            b: "What",
            c: "Am",
            d: "I doing here?",
          },
          {
            a: "¿Qué tan rápido puedes caminar en el barro?",
            b: "How fast",
            c: "Can",
            d: "You walk in the mud?",
          },
          {
            a: "¿Cuánto tiempo ella ha estado casada con él?",
            b: "How long",
            c: "Has",
            d: "She been married to him?",
          },
          {
            a: "¿Cómo has estado?",
            b: "How",
            c: "Have",
            d: "you been?",
          },
          {
            a: "¿A qué horas deberías apagar esto?",
            b: "What time",
            c: "Should",
            d: "I turn this off?",
          },
          {
            a: "¿Qué debemos hacer ahora?",
            b: "What",
            c: "Must",
            d: "We do now?",
          },
          {
            a: "¿Cuándo fue la última vez has viajado?",
            b: "When",
            c: "Was",
            d: "The last time you travelled?",
          },
          {
            a: "¿Por qué estabas gritando fuerte?",
            b: "Why",
            c: "Were",
            d: "You screaming loudly?",
          },
          {
            a: "¿Qué tan lejos podríamos llegar desde aquí?",
            b: "How far",
            c: "Could",
            d: "We get from here?",
          },
          {
            a: "¿Cuánto tiempo habías estado esperando?",
            b: "How long",
            c: "Have",
            d: "You been waiting for him?",
          },
          {
            a: "¿Cómo puedo ayudarte?",
            b: "How",
            c: "May",
            d: "I help you?",
          },
          {
            a: "¿Dónde podríamos dormir esta noche?",
            b: "Where",
            c: "Might",
            d: "we sleep tonight?",
          },
        ],
      },
    };
  },
};
</script>
