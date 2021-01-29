<template>
  <div>
    <b-container fluid>
      <b-row>
        <b-col></b-col>
        <b-col sm="auto">
          <h3 class="titulo">SUB + VERB + OBJECT + TO VERB</h3>
        </b-col>
        <b-col></b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            Esta estructura tiene tres novedades
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            <b>1. </b>Algunas veces el primer verbo tiene la palabra “que”. Por
            ejemplo: me gusta “que” ella conduzca (I like her to drive). Aunque
            en inglés el verbo lleva la palabra “que” incluida.
          </h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            <b>2. </b>Otras oraciones tienen la palabra “que” en el segundo
            verbo. Por ejemplo: el comandante les ordenó a los soldados que se
            retiraran. (the commander ordered the soldiers to withdraw).
          </h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            <b>3. </b>La forma negativa es usar la palabra “not” antes del
            segundo verbo. Por ejemplo: ella me pidió que no fuera. (she asked
            me not to go)
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="11">
          <h3 class="subTitulo">EXAMPLES</h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            <b>Advise: </b>I want you to advise me on what is the right English
            academy for me. <br /><br />
            <b>Allow: </b>I said not to allow him to leave the class.
            <br /><br />
            <b>Ask:</b>She thought you wanted to ask her to marry you.
            <br /><br />
            <b>Beg: </b>My parents reminded me to beg for forgiveness.
            <br /><br />
            <b>Cause: </b>She asked me not to cause trouble. <br /><br />
            <b>Choose: </b>I said to choose either him or me. <br /><br />
            <b>Convince: </b>I need to convince her to buy me some shoes.
            <br /><br />
            <b>Enable: </b>I tried not to enable his addiction. <br /><br />
            <b>Encourage: </b>They said not to encourage his bad behaviour.
            <br /><br />
            <b>Command: </b>I wanted him to command the class to be quiet.
            <br /><br />
            <b>Persuade: </b>She demands that I try to persuade the shop
            assistant to lower the price. <br /><br />
            <b>Expect: </b>Please tell John not to expect good news today.
            <br /><br />
            <b>Force: </b>My personal trainer said I need to force myself to
            exercise because I’m so lazy. <br /><br />
            <b>Instruct: </b>He showed me how to instruct the other students how
            to learn. <br /><br />
            <b>Invite: </b>My mum said to invite Daryl to the party, even though
            I don’t like him. <br /><br />
            <b>Need: </b>I learnt not to need sugar in my diet. <br /><br />
            <b>Order: </b>I sent a letter to order him to stop immediately.
            <br /><br />
            <b>Permit: </b>I needed her to permit me to use the computer.
            <br /><br />
            <b>Prepare: </b>I showed him how to prepare the cake. <br /><br />
            <b>Promise: </b>I warned him not to promise something he couldn’t
            keep. <br /><br />
            <b>Hire: </b>Please remind me to hire Victor as my bodyguard.
            <br /><br />
            <b>Threaten: </b>Tell him not to threaten me. <br /><br />
            <b>Remind: </b>I have my phone set up to remind me when it’s our
            anniversary. <br /><br />
            <b>Require: </b>I learnt not to require anybody’s help. <br /><br />
            <b>Tell: </b>She asked me not to tell her secret to anyone!
            <br /><br />
            <b>Urge: </b>She has arrived to urge me to give her some money.
            <br /><br />
            <b>Want: </b>To win this competition you need to want to win!
            <br /><br />
            <b>Warn: </b>Did you tell her to warn me about the dangerous dog?
            <br /><br />
            <b>Wish: </b>I know not to wish for anything on your birthday,
            because wishes never come true. <br /><br />
            <b>Would like: </b>I would like you to be quiet.
          </h3>
        </b-col>
      </b-row>

      <br />
      <b-row>
        <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            Complete with the most suitable verb
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            <b>1. </b> My mom told <span class="colorLetraRojo">me</span>
          </h3>
        </b-col>

        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['to make']"
            tamano="12.3"
          />
        </b-col>

        <b-col sm="4">
          <h3 class="parrafoIC">chicken for dinner.</h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            <b>2. </b> Her boyfriend asked
            <span class="colorLetraRojo">her</span>
          </h3>
        </b-col>

        <b-col sm="left">
          <inputChecked :resuelto="false" :esperado="['to pay']" tamano="11" />
        </b-col>

        <b-col sm="4">
          <h3 class="parrafoIC">his phone bill.</h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            <b>3. </b> Ethan wanted <span class="colorLetraRojo">me</span>
          </h3>
        </b-col>

        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['to teach']"
            tamano="12.3"
          />
        </b-col>

        <b-col sm="4">
          <h3 class="parrafoIC">him how to dance.</h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            <b>4. </b> The traffic officer warned
            <span class="colorLetraRojo">me not</span>
          </h3>
        </b-col>

        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['to drive']"
            tamano="11.5"
          />
        </b-col>

        <b-col sm="5">
          <h3 class="parrafoIC">too quickly because of the bad weather.</h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            <b>5. </b>I always remind
            <span class="colorLetraRojo">my son </span>
          </h3>
        </b-col>

        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['to set']"
            tamano="12.3"
          />
        </b-col>

        <b-col sm="4">
          <h3 class="parrafoIC">the alarm at 6.</h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            <b>6. </b>Please tell <span class="colorLetraRojo">him not </span>
          </h3>
        </b-col>

        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['to smoke']"
            tamano="12.3"
          />
        </b-col>

        <b-col sm="4">
          <h3 class="parrafoIC">here. – this is a non-smoking room.</h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            <b>7. </b>I didn't feel too good but my friends persuaded<span
              class="colorLetraRojo"
              >me</span
            >
          </h3>
        </b-col>

        <b-col sm="left">
          <inputChecked :resuelto="false" :esperado="['to go']" tamano="12.3" />
        </b-col>

        <b-col sm="3">
          <h3 class="parrafoIC">to the party.</h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            <b>8. </b>Nobody wanted to leave but the circumstances forced
            <span class="colorLetraRojo">us</span>
          </h3>
        </b-col>

        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['to leave']"
            tamano="12.3"
          />
        </b-col>

        <b-col sm="3">
          <h3 class="parrafoIC">it.</h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            <b>9. </b>I asked Michael <span class="colorLetraRojo">not</span>
          </h3>
        </b-col>

        <b-col sm="left">
          <inputChecked :resuelto="false" :esperado="['to call']" tamano="11" />
        </b-col>

        <b-col sm="6">
          <h3 class="parrafoIC">
            <span class="colorLetraRojo">me</span> so late in the evening
            because I always turn my phone
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3>
            off when sleeping.
          </h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            <b>10. </b>They showed <span class="colorLetraRojo">us how</span>
          </h3>
        </b-col>

        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['to use']"
            tamano="12.3"
          />
        </b-col>

        <b-col sm="4">
          <h3 class="parrafoIC">the new equipment.</h3>
        </b-col>
      </b-row>
      <br /><br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="7">
          <tablaTC :cuestionario="tabla4P7" />
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <tablaTC :cuestionario="tabla5P7" />
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            Write down the pronoun plus the verb to complete the phrase.
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="10">
          <tablaTC :cuestionario="tabla7P7" />
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
      tabla7P7: {
        fields: [
          { key: "a", label: "" },
          { key: "complejo1", label: "VERB + OBJECT + TO VERB" },
        ],
        items: [
          {
            a: "¿Qué quieres que yo haga?",
            complejo1: {
              lista: ["me to do"],
              conTexto: true,
              textoA: "What do you want",
              textoD: "?",
              tamano: 27,
              resuelto: false,
            },
          },
          {
            a: "¿Ella dónde quiere que nosotros durmamos?",
            complejo1: {
              lista: ["us to sleep"],
              conTexto: true,
              textoA: "Where does she want",
              textoD: "?",
              tamano: 30.5,
              resuelto: false,
            },
          },
          {
            a: "¿Cuándo te gustaría que lo llamáramos?",
            complejo1: {
              lista: ["us to call him"],
              conTexto: true,
              textoA: "When would you like",
              textoD: "?",
              tamano: 31,
              resuelto: false,
            },
          },
          {
            a: "¿Porque quieres que yo me vaya?",
            complejo1: {
              lista: ["me to leave"],
              conTexto: true,
              textoA: "Why do you want",
              textoD: "?",
              tamano: 28,
              resuelto: false,
            },
          },
          {
            a: "¿Qué te gusta que nosotros hagamos?",
            complejo1: {
              lista: ["us to do"],
              conTexto: true,
              textoA: "What would you like",
              textoD: "?",
              tamano: 28,
              resuelto: false,
            },
          },
          {
            a: "¿Porque ella quiere que él se vaya?",
            complejo1: {
              lista: ["she want him to leave"],
              conTexto: true,
              textoA: "Why does",
              textoD: "?",
              tamano: 29,
              resuelto: false,
            },
          },
          {
            a: "¿Ella que necesita que ellos digan?",
            complejo1: {
              lista: ["she need them to say"],
              conTexto: true,
              textoA: "What does ",
              textoD: "?",
              tamano: 29.3,
              resuelto: false,
            },
          },
          {
            a: "¿Dónde quieres que yo duerma?",
            complejo1: {
              lista: ["you want me to sleep"],
              conTexto: true,
              textoA: "Where do ",
              textoD: "?",
              tamano: 28.4,
              resuelto: false,
            },
          },
          {
            a: "Yo quiero que tú me entiendas.",
            complejo1: {
              lista: ["you to understand me"],
              conTexto: true,
              textoA: "I want",
              textoD: "",
              tamano: 25.3,
              resuelto: false,
            },
          },
          {
            a: "No queremos que nuestro hijo se sienta mal.",
            complejo1: {
              lista: ["our son to feel bad"],
              conTexto: true,
              textoA: "We don´t want ",
              textoD: "",
              tamano: 29.3,
              resuelto: false,
            },
          },
          {
            a: "Disfruto que los niños jueguen en mi casa",
            complejo1: {
              lista: ["playing at my house"],
              conTexto: true,
              textoA: "I enjoy the kids ",
              textoD: "",
              tamano: 30.3,
              resuelto: false,
            },
          },
          {
            a: "Necesito que me digas qué está pasando",
            complejo1: {
              lista: ["to tell me "],
              conTexto: true,
              textoA: "I need you ",
              textoD: "what´s going on",
              tamano: 32,
              resuelto: false,
            },
          },
        ],
      },
      tabla5P7: {
        fields: [
          { key: "a", label: "", thClass: "Yelow" },
          { key: "b", label: "", thClass: "Blue" },
          { key: "c", label: "", thClass: "Green" },
          { key: "d", label: "", thClass: "Pink" },
          { key: "e", label: "", thClass: "Red" },
          { key: "complejo1", label: "English" },
          { key: "g", label: "Spanish" },
        ],
        items: [
          {
            a: "3",
            b: "1",
            c: "1",
            d: "1",
            e: "7",
            complejo1: {
              lista: ["We want them to listen to us"],
              tamano: 25,
              resuelto: false,
            },
            g: "Nosotros queremos que ellos nos escuchen",
          },
          {
            a: "2",
            b: "2",
            c: "2",
            d: "2",
            e: "2",
            complejo1: {
              lista: ["She doesn’t like anybody to bother her"],
              tamano: 31,
              resuelto: false,
            },
            g: "A ella no le gusta que nadie la moleste",
          },
          {
            a: "5",
            b: "1",
            c: "5",
            d: "5",
            e: "5",
            complejo1: {
              lista: ["What do you want me to tell you?"],
              tamano: 28,
              resuelto: false,
            },
            g: "¿Qué quieres que yo te diga?",
          },
          {
            a: "4",
            b: "4",
            c: "4",
            d: "4",
            e: "4",
            complejo1: {
              lista: ["He needs his girlfriend to call him"],
              tamano: 28,
              resuelto: false,
            },
            g: "Él necesita que su novia lo llame",
          },
          {
            a: "4",
            b: "4",
            c: "7",
            d: "7",
            e: "4",
            complejo1: {
              lista: ["He needs us to help him"],
              tamano: 23,
              resuelto: false,
            },
            g: "Él necesita que nosotros lo ayudemos",
          },
          {
            a: "6",
            b: "5",
            c: "2",
            d: "7",
            e: "1",
            complejo1: {
              lista: ["I don’t need anybody to help me"],
              tamano: 27.3,
              resuelto: false,
            },
            g: "Yo no necesito que nadie me ayude",
          },
          {
            a: "1",
            b: "1",
            c: "6",
            d: "1",
            e: "2",
            complejo1: {
              lista: ["I want you to listen to her"],
              tamano: 23.5,
              resuelto: false,
            },
            g: "Yo quiero que tú la escuches",
          },
          {
            a: "7",
            b: "3",
            c: "3",
            d: "2",
            e: "6",
            complejo1: {
              lista: ["They hate our mother to bother them"],
              tamano: 30,
              resuelto: false,
            },
            g: "Ellos odian que nuestra madre los moleste",
          },
          {
            a: "3",
            b: "7",
            c: "3",
            d: "3",
            e: "3",
            complejo1: {
              lista: ["We asked our mother to wake us up"],
              tamano: 30,
              resuelto: false,
            },
            g: "Nosotros le pedimos a  nuestra madre que nos despertara",
          },
          {
            a: "6",
            b: "5",
            c: "2",
            d: "8",
            e: "8",
            complejo1: {
              lista: ["I don’t need anybody to tell me what to do"],
              tamano: 33,
              resuelto: false,
            },
            g: "Yo no necesito que nadie me diga que hacer",
          },
          {
            a: "2",
            b: "1",
            c: "6",
            d: "4",
            e: "2",
            complejo1: {
              lista: ["She doesn’t want you to call her"],
              tamano: 28,
              resuelto: false,
            },
            g: "Ella no quiere que tú la llames",
          },
          {
            a: "1",
            b: "6",
            c: "1",
            d: "7",
            e: "1",
            complejo1: {
              lista: ["I love them to help me"],
              tamano: 22,
              resuelto: false,
            },
            g: "Yo amo que ellos me ayuden",
          },
          {
            a: "1",
            b: "7",
            c: "1",
            d: "7",
            e: "1",
            complejo1: {
              lista: ["I asked them to help me"],
              tamano: 23,
              resuelto: false,
            },
            g: "Yo les pedí que me ayuden",
          },
        ],
      },
      tabla4P7: {
        fields: [
          { key: "a", label: "Subject", thClass: "Yelow" },
          { key: "b", label: "Verb", thClass: "Blue" },
          { key: "c", label: "Object", thClass: "Green" },
          { key: "d", label: "Verb", thClass: "Pink" },
          { key: "e", label: "Object", thClass: "Red" },
        ],
        items: [
          {
            a: "1. I",
            b: "1. want",
            c: "1. them",
            d: "1. to listen to",
            e: "1. me",
          },
          {
            a: "2. She doesn ́t",
            b: "2. like",
            c: "2. anybody",
            d: "2. to bother",
            e: "2. her",
          },
          {
            a: "3. We",
            b: "3. hate",
            c: "3. our mother",
            d: "3. to wake",
            e: "3. us up",
          },
          {
            a: "4. He",
            b: "4. needs",
            c: "4. his girlfriend",
            d: "4. to call",
            e: "4. him",
          },
          {
            a: "5. What do you",
            b: "5. Need",
            c: "5. me",
            d: "5. to tell",
            e: "5. you",
          },
          {
            a: "6. I don ́t",
            b: "6. love",
            c: "6. you",
            d: "6. to respet",
            e: "6. them",
          },
          {
            a: "7. They",
            b: "7. asked",
            c: "7. us",
            d: "7. to help",
            e: "7. us",
          },
          {
            d: "8. to tell me",
            e: "8. what to do",
          },
        ],
      },
    };
  },
};
</script>
