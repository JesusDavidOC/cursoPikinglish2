<template>
  <b-container fluid>
    <b-row>
      <b-col></b-col>
      <b-col sm="auto">
        <h3 class="titulo">HOW TO USE THE SUFFIX “ED”.</h3>
      </b-col>
      <b-col></b-col>
    </b-row>
    <b-row>
      <b-col></b-col>
      <b-col sm="8">
        <p class="parrafo">
          As we know there are a lot of English irregular verbs that have a
          different spelling form in the past tense as well as in participle,
          however we have listed them in groups.
        </p>
      </b-col>
      <b-col></b-col>
    </b-row>
    <b-row class="diamondContainer">
      <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
      <b-col>
        <h3 class="fuenteDiamond">
          First group: Written the same way in all tenses.
        </h3>
      </b-col>
    </b-row>
    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="auto">
        <tablaTC id="tabla1P10" :cuestionario="tabla1P10" />
      </b-col>
    </b-row>
    <b-row class="diamondContainer">
      <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
      <b-col>
        <h3 class="fuenteDiamond">
          Second group. Ending in <span class="colorLetraRojo">GHT</span> in the
          past and as well as in participle.
        </h3>
      </b-col>
    </b-row>
    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="auto">
        <tablaTC id="tabla1P11" :cuestionario="tabla1P11" />
      </b-col>
    </b-row>
    <b-row class="diamondContainer">
      <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
      <b-col>
        <h3 class="fuenteDiamond">
          Third group: Those ending in <span class="colorLetraRojo">EN</span>
          in the participle form.
        </h3>
      </b-col>
    </b-row>
    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="auto">
        <tablaTC id="tabla2P11" :cuestionario="tabla2P11" />
      </b-col>
    </b-row>

    <b-row class="diamondContainer">
      <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
      <b-col>
        <h3 class="fuenteDiamond">
          Fourth group: Verbs spelled the same as in the past as well as in
          participle
        </h3>
      </b-col>
    </b-row>
    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="auto">
        <tablaTC id="tabla1P12" :cuestionario="tabla1P12" />
      </b-col>
    </b-row>
    <b-row class="diamondContainer">
      <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
      <b-col>
        <h3 class="fuenteDiamond">
          Fifth group: The vowel changes in all three forms. I, A, U
        </h3>
      </b-col>
    </b-row>
    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="auto">
        <tablaTC id="tabla1P13" :cuestionario="tabla1P13" />
      </b-col>
    </b-row>

    <b-row class="diamondContainer">
      <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
      <b-col>
        <h3 class="fuenteDiamond">
          Sixth group: Past tense ending in ew and participle verbs ending in wn
        </h3>
      </b-col>
    </b-row>
    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="auto">
        <tablaTC id="tabla2P13" :cuestionario="tabla2P13" />
      </b-col>
    </b-row>
    <b-row class="diamondContainer">
      <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
      <b-col>
        <h3 class="fuenteDiamond">
          Seventh group: Present form is spelled the same as participle.
        </h3>
      </b-col>
    </b-row>
    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="auto">
        <tablaTC id="tabla1P14" :cuestionario="tabla1P14" />
      </b-col>
    </b-row>

    <b-row class="diamondContainer">
      <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
      <b-col>
        <h3 class="fuenteDiamond">
          Eighth group: Ending in <span class="colorLetraRojo">re</span> in past
          and in <span class="colorLetraRojo">rn</span> in participle.
        </h3>
      </b-col>
    </b-row>
    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="auto">
        <tablaTC id="tabla2P14" :cuestionario="tabla2P14" />
      </b-col>
    </b-row>

    <b-row class="diamondContainer">
      <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
      <b-col>
        <h3 class="fuenteDiamond">Ninth group: Other irregular verbs.</h3>
      </b-col>
    </b-row>
    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="auto">
        <tablaTC id="tabla3P14" :cuestionario="tabla3P14" />
      </b-col>
    </b-row>

    <b-row class="diamondContainer">
      <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
      <b-col>
        <h3 class="fuenteDiamond">
          Answer the following questions with verbs in the past.
        </h3>
      </b-col>
    </b-row>
    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="auto">
        <b-row
          v-for="(item, index) in listadoInputsP15"
          :key="'listadoInputsP15' + index"
        >
          <b-row>
            <h4>
              <strong>{{ item.pregunta }}</strong>
            </h4>
          </b-row>
          <b-row> </b-row>
            <inputChecked
              :esperado="item.esperado"
              :tamano="item.tamano-1"
              :conTexto="true"
              :textoA="item.textoA"
              :textoD="item.textoD"
              :textoD2="item.textoD2"
            />
          
        </b-row>
      </b-col>
    </b-row>
    <b-row class="diamondContainer">
      <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
      <b-col>
        <h3 class="fuenteDiamond">THE BEST DAY EVER</h3>
      </b-col>
    </b-row>
    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="4">
        <tablaTC id="tabla1P15" :cuestionario="tabla1P15" />
      </b-col>
    </b-row>

    <b-row class="diamondContainer">
      <b-col sm="1"></b-col>
      <b-col sm="10">
        <audioComp :elemento="elementoTextP16" />
      </b-col>
    </b-row>
    <b-row>
      <b-col>
        <h3 class="subTitulo">QUESTIONS</h3>
      </b-col>
    </b-row>
    <b-row>
      <b-col sm="1"></b-col>
      <b-col>
        <opcionMultiple :object="oMultipleP16" />
      </b-col>
    </b-row>

    <b-row class="diamondContainer">
      <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
      <b-col>
        <h3 class="fuenteDiamond">Complete the phrase, listen and complete</h3>
      </b-col>
    </b-row>
    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="10">
        <tablaTC id="tabla1P17" :cuestionario="tabla1P17" />
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
import posiblesRespuestasTabla from "./posiblesRespuestasTabla";
import opcionMultiple from "./opcionMultiple";
import listaIndex from "./listaIndex";
import inputChecked from "./inputChecked";
import tablaTC from "./tablaTraduccionCodigos";
import audioComp from "./audioComp";
export default {
  components: {
    tablaTC,
    opcionMultiple,
    inputChecked,
    audioComp,
  },
  data() {
    return {
      tabla1P17: {
        fields: [
          { key: "a", thClass: "noHead" },
          { key: "complejo1", thClass: "noHead" },
        ],
        items: [
          {
            a: "Desayuné con ellos",
            complejo1: {
              lista: ["took"],
              textoA: "I",
              textoD: "breakfast with them",
              tamano: 20,
            },
          },
          {
            a: "Dejé la Puerta abierta",
            complejo1: {
              lista: ["left"],
              textoA: "I",
              textoD: "the door open",
              tamano: 15.5,
            },
          },
          {
            a: "Escribí mi nombre en la pared",
            complejo1: {
              lista: ["wrote"],
              textoA: "I",
              textoD: "my name on the wall",
              tamano: 21,
            },
          },
          {
            a: "La vi bailando",
            complejo1: {
              lista: ["saw"],
              textoA: "I",
              textoD: "her dancing",
              tamano: 14.3,
            },
          },
          {
            a: "Lo hiciste bien",
            complejo1: {
              lista: ["did"],
              textoA: "You",
              textoD: "it well",
              tamano: 12,
            },
          },
          {
            a: "Salí con el",
            complejo1: {
              lista: ["went"],
              textoA: "I",
              textoD: "out with him ",
              tamano: 15,
            },
          },
          {
            a: "Ellos nos llevaron allá",
            complejo1: {
              lista: ["took"],
              textoA: "They",
              textoD: "us there ",
              tamano: 15,
            },
          },
          {
            a: "Nadie me contó",
            complejo1: {
              lista: ["found"],
              textoA: "Nobody",
              textoD: "me",
              tamano: 13.7,
            },
          },
          {
            a: "Todos sabían de ello",
            complejo1: {
              lista: ["knew"],
              textoA: "Everybody",
              textoD: "about it",
              tamano: 19,
            },
          },
          {
            a: "Nosotros sostuvimos la fiesta en la escuela",
            complejo1: {
              lista: ["held"],
              textoA: "We",
              textoD: "the party at the school ",
              tamano: 23.3,
            },
          },
          {
            a: "Pensé que sería difícil ",
            complejo1: {
              lista: ["thought"],
              textoA: "I",
              textoD: "it would be hard",
              tamano: 19,
            },
          },
          {
            a: "Compré un par de medias",
            complejo1: {
              lista: ["bought"],
              textoA: "I",
              textoD: "a pair of socks",
              tamano: 18,
            },
          },
          {
            a: "Entendimos perfectamente",
            complejo1: {
              lista: ["understood"],
              textoA: "We",
              textoD: "perfectly ",
              tamano: 18,
            },
          },
          {
            a: "Todos nosotros dormimos bien",
            complejo1: {
              lista: ["slept"],
              textoA: "We all",
              textoD: "very well",
              tamano: 16.5,
            },
          },
          {
            a: "Me sentí un poco extraño",
            complejo1: {
              lista: ["felt"],
              textoA: "I",
              textoD: "a bit weird",
              tamano: 13,
            },
          },
          {
            a: "Nos conocimos hace mucho tiempo",
            complejo1: {
              lista: ["met"],
              textoA: "We",
              textoD: "a very long time ago",
              tamano: 22,
            },
          },
          {
            a: "Le vendi mi carro a él",
            complejo1: {
              lista: ["selt"],
              textoA: "I",
              textoD: "him my car",
              tamano: 14,
            },
          },
          {
            a: "Ellos me enviaron una tarjeta",
            complejo1: {
              lista: ["sent"],
              textoA: "They",
              textoD: "me a post card",
              tamano: 19.5,
            },
          },
          {
            a: "Ella me prestó algo de dinero",
            complejo1: {
              lista: ["lent"],
              textoA: "I",
              textoD: "me some money",
              tamano: 17.5,
            },
          },
          {
            a: "Nunca he enseñado",
            complejo1: {
              lista: ["taught"],
              textoA: "I have never",
              tamano: 16,
            },
          },
          {
            a: "No he colgado el cuadro aún",
            complejo1: {
              lista: ["hung"],
              textoA: "I haven’t",
              textoD: "the painting yet",
              tamano: 23,
            },
          },
          {
            a: "Ella me lanzó el balón",
            complejo1: {
              lista: ["threw"],
              textoA: "She",
              textoD: "the ball to me",
              tamano: 19,
            },
          },
          {
            a: "Ella habló con la policía",
            complejo1: {
              lista: ["spoke"],
              textoA: "she",
              textoD: "to the police",
              tamano: 17.7,
            },
          },
          {
            a: "Ellos me dieron esto",
            complejo1: {
              lista: ["gave"],
              textoA: "They",
              textoD: "me this",
              tamano: 15,
            },
          },
          {
            a: "He tenido un gran día",
            complejo1: {
              lista: ["got"],
              textoA: "I have",
              textoD: "a great day",
              tamano: 17.2,
            },
          },
          {
            a: "Atrapé un resfriado",
            complejo1: {
              lista: ["caught"],
              textoA: "I",
              textoD: "a cold",
              tamano: 12,
            },
          },
          {
            a: "Nadie ha traído nada",
            complejo1: {
              lista: ["brought"],
              textoA: "Nobody has",
              textoD: "anything",
              tamano: 22,
            },
          },
          {
            a: "Ella finalmente me perdonó",
            complejo1: {
              lista: ["finally"],
              textoA: "She",
              textoD: "forgave me",
              tamano: 17.5,
            },
          },
          {
            a: "He conducido durante 5 horas",
            complejo1: {
              lista: ["drove"],
              textoA: "I have",
              textoD: "for 5 hours",
              tamano: 18.5,
            },
          },
          {
            a: "Encendí una vela",
            complejo1: {
              lista: ["lit"],
              textoA: "I",
              textoD: "a candle",
              tamano: 11,
            },
          },
          {
            a: "He volado a España dos veces",
            complejo1: {
              lista: ["flew"],
              textoA: "I have",
              textoD: "to Spain twice ",
              tamano: 19.5,
            },
          },
          {
            a: "Él se volvió profesor",
            complejo1: {
              lista: ["became"],
              textoA: "He",
              textoD: "a teacher ",
              tamano: 16.5,
            },
          },
        ],
      },
      oMultipleP16: {
        rEsperadas: ["B", "A", "C", "B"],
        options: [
          {
            respuesta: "",
            pregunta: "1.	What was my mum wearing when she came into my room?",
            options: [
              { text: "A strange dress", value: "A" },
              { text: "A chicken costume", value: "B" },
              { text: "A funny way", value: "C" },
            ],
          },
          {
            respuesta: "",
            pregunta: "2.	What did Ronaldo offer to buy me?",
            options: [
              { text: "A new pair of flip flops", value: "A" },
              { text: "My shopping", value: "B" },
              { text: "A football", value: "C" },
            ],
          },
          {
            respuesta: "",
            pregunta: "3.	How much money did I find?",
            options: [
              { text: "Twenty dollars", value: "A" },
              { text: "Twenty thousand dollars", value: "B" },
              { text: "Two hundred dollars", value: "C" },
            ],
          },
          {
            respuesta: "",
            pregunta: "4.	What did I shout when I got home?",
            options: [
              { text: "I ran inside", value: "A" },
              { text: "Mom, today was the best day ever", value: "B" },
              { text: "About my day", value: "C" },
            ],
          },
        ],
      },
      elementoTextP16: {
        audio: "/cursos/curso2/leccion3/audios/page15/audioC2P15E2P1.mp3",
        textoD:
          "Yesterday was the best day ever! The day <strong>began</strong> a little strange, but in a funny way. My mom <strong>came</strong> into my room, to wake me up, wearing a chicken costume. When I <strong>woke</strong> up, I thought I was dreaming! After, I <strong>went</strong> to run some errands. On my way to the supermarket, a man <strong>ran</strong> into me. When I <strong>looked</strong> up to see who it was, I couldn’t believe my eyes. It was Cristiano Ronaldo! When he <strong>noticed</strong> he broke my flip flop, he <strong>offered</strong> to buy a new pair. I was so nervous, I quickly replied, “uh... it is ok! I <strong>bought</strong> them a long time ago” and <strong>ran</strong> away. Then, just as I <strong>got</strong> to the supermarket, I <strong>realized</strong> I <strong>forgot</strong> my money! I felt so frustrated I <strong>fell</strong> to my knees crying. When I <strong>looked</strong> up, I <strong>saw</strong> $200 laying in the grass. I <strong>went</strong> into the store and <strong>bought</strong> a lot of food. After, I <strong>went</strong> home to tell my mom about my day. I <strong>ran</strong> inside and <strong>shouted</strong> “MOM, TODAY WAS THE BEST DAY EVER!”",
      },
      tabla1P15: {
        fields: [
          { key: "complejoAudio1", thClass: "noHead" },
          { key: "b", thClass: "noHead" },
        ],
        items: [
          {
            complejoAudio1: {
              textoA: "Strange",
              audio: "/cursos/curso2/leccion3/audios/page15/audioC2P15E1P1.mp3",
              tamano: 13,
            },
            b: "Extraño",
          },
          {
            complejoAudio1: {
              textoA: "Funny",
              audio: "/cursos/curso2/leccion3/audios/page15/audioC2P15E1P2.mp3",
              tamano: 13,
            },
            b: "Divertido",
          },
          {
            complejoAudio1: {
              textoA: "Errands",
              audio: "/cursos/curso2/leccion3/audios/page15/audioC2P15E1P3.mp3",
              tamano: 13,
            },
            b: "Mandado",
          },
          {
            complejoAudio1: {
              textoA: "Flip Flop",
              audio: "/cursos/curso2/leccion3/audios/page15/audioC2P15E1P4.mp3",
              tamano: 13,
            },
            b: "Chancleta",
          },
          {
            complejoAudio1: {
              textoA: "Knees",
              audio: "/cursos/curso2/leccion3/audios/page15/audioC2P15E1P5.mp3",
              tamano: 13,
            },
            b: "Rodillas",
          },
          {
            complejoAudio1: {
              textoA: "Inside",
              audio: "/cursos/curso2/leccion3/audios/page15/audioC2P15E1P6.mp3",
              tamano: 13,
            },
            b: "Adentro",
          },
        ],
      },
      listadoInputsP15: [
        {
          esperado: ["Bought"],
          pregunta: "1.	What did you buy?",
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
        {
          esperado: ["said"],
          pregunta: "16.	What did you say to me?",
          textoA: "I",
          textoD: "you're beautiful.",
          tamano: 19,
        },
        {
          esperado: ["forgave"],
          pregunta: "17.	Will you ever forgive him?",
          textoA: "I",
          textoD: "him yesterday.",
          tamano: 19.9,
        },
        {
          esperado: ["woke"],
          pregunta: "18.	What time do you normally wake up?",
          textoA: "Well, this morning I",
          textoD: "up at 10am, but normally",
          textoD2: "I wake up at 7am.",
          tamano: 37.8,
        },
        {
          esperado: ["hid"],
          pregunta: "19.	Where did you hide when that man came into your room?",
          textoA: "I",
          textoD: "under the bed!",
          tamano: 17.5,
        },
        {
          esperado: ["thought"],
          pregunta: "20.	What did you think was going to happen?",
          textoA: "I",
          textoD: "she’d say yes and we’d live happily ever after.",
          tamano: 41,
        },
      ],
      tabla3P14: {
        fields: [
          { key: "a", label: "Present", thClass: "colorLetraRojo" },
          { key: "b", label: "Past", thClass: "colorLetraRojo" },
          { key: "c", label: "Participle ", thClass: "colorLetraRojo" },
          { key: "d", label: "Translation ", thClass: "colorLetraRojo" },
        ],
        items: [
          { a: "Get", b: "Got", c: "Gotten/got", d: "Conseguir." },
          { a: "Go", b: "Went", c: "Gone", d: "Ir." },
          { a: "Do", b: "Did", c: "Done", d: "Hacer." },
          { a: "Lie", b: "Lay", c: "Lain", d: "Acostarse." },
        ],
      },
      tabla2P14: {
        fields: [
          { key: "a", label: "Present", thClass: "colorLetraRojo" },
          { key: "html1", label: "Past", thClass: "colorLetraRojo" },
          { key: "html2", label: "Participle ", thClass: "colorLetraRojo" },
          { key: "b", label: "Translation ", thClass: "colorLetraRojo" },
        ],
        items: [
          {
            a: "Swear",
            html1: "Swo<span class='colorLetraRojo'>re</span>",
            html2: "Swo<span class='colorLetraRojo'>rn</span>",
            b: "Jurar.",
          },
          {
            a: "Wear",
            html1: "Wo<span class='colorLetraRojo'>re</span>",
            html2: "Wo<span class='colorLetraRojo'>rn</span>",
            b: "Usar.",
          },
          {
            a: "Tear",
            html1: "To<span class='colorLetraRojo'>re</span>",
            html2: "To<span class='colorLetraRojo'>rn</span>",
            b: "Arrancar.",
          },
          {
            a: "Bear",
            html1: "Bo<span class='colorLetraRojo'>re</span>",
            html2: "Bo<span class='colorLetraRojo'>rn</span>",
            b: "Soportar.",
          },
        ],
      },
      tabla1P14: {
        fields: [
          { key: "a", label: "Present", thClass: "colorLetraRojo" },
          { key: "b", label: "Past", thClass: "colorLetraRojo" },
          { key: "c", label: "Participle ", thClass: "colorLetraRojo" },
          { key: "d", label: "Translation ", thClass: "colorLetraRojo" },
        ],
        items: [
          { a: "Come", b: "Came", c: "Come", d: "Venir." },
          { a: "Become", b: "Became", c: "Become", d: "Volverse." },
          { a: "Run", b: "Ran", c: "Run", d: "Correr." },
        ],
      },
      tabla2P13: {
        fields: [
          { key: "a", label: "Present", thClass: "colorLetraRojo" },
          { key: "html2", label: "Past", thClass: "colorLetraRojo" },
          { key: "html3", label: "Participle ", thClass: "colorLetraRojo" },
          { key: "b", label: "Translation ", thClass: "colorLetraRojo" },
        ],
        items: [
          {
            a: "Blow",
            html2:
              "<span class='colorLetraAzul'>Bl<span class='colorLetraRojo'>ew</span></span>",
            html3:
              "<span class='colorLetraAzul'>Blo<span class='colorLetraRojo'>wn</span></span>",
            b: "Soplar.",
          },
          {
            a: "Fly",
            html2:
              "<span class='colorLetraAzul'>Fl<span class='colorLetraRojo'>ew</span></span>",
            html3:
              "<span class='colorLetraAzul'>Flo<span class='colorLetraRojo'>wn</span></span>",
            b: "Volar.",
          },
          {
            a: "Throw",
            html2:
              "<span class='colorLetraAzul'>Thr<span class='colorLetraRojo'>ew</span></span>",
            html3:
              "<span class='colorLetraAzul'>Thro<span class='colorLetraRojo'>wn</span></span>",
            b: "Lanzar.",
          },
          {
            a: "Draw",
            html2:
              "<span class='colorLetraAzul'>Dr<span class='colorLetraRojo'>ew</span></span>",
            html3:
              "<span class='colorLetraAzul'>Blo<span class='colorLetraRojo'>wn</span></span>",
            b: "Dibujar.",
          },

          {
            a: "Grow",
            html2:
              "<span class='colorLetraAzul'>Gr<span class='colorLetraRojo'>ew</span></span>",
            html3:
              "<span class='colorLetraAzul'>Gro<span class='colorLetraRojo'>wn</span></span>",
            b: "Sembrar-crecer.",
          },

          {
            a: "Know",
            html2:
              "<span class='colorLetraAzul'>Kn<span class='colorLetraRojo'>ew</span></span>",
            html3:
              "<span class='colorLetraAzul'>Kno<span class='colorLetraRojo'>wn</span></span>",
            b: "Saber.",
          },
        ],
      },
      tabla1P13: {
        fields: [
          { key: "html1", label: "Present", thClass: "colorLetraRojo" },
          { key: "html2", label: "Past", thClass: "colorLetraRojo" },
          { key: "html3", label: "Participle ", thClass: "colorLetraRojo" },
          { key: "d", label: "Translation ", thClass: "colorLetraRojo" },
        ],
        items: [
          {
            html1: "Beg<span class='colorLetraRojo'>i</span>n",
            html2: "Beg<span class='colorLetraRojo'>a</span>n",
            html3: "Beg<span class='colorLetraRojo'>u</span>n",
            d: "Iniciar.",
          },
          {
            html1: "S<span class='colorLetraRojo'>i</span>ng",
            html2: "S<span class='colorLetraRojo'>a</span>ng",
            html3: "S<span class='colorLetraRojo'>u</span>ng",
            d: "Cantar.",
          },
          {
            html1: "R<span class='colorLetraRojo'>i</span>ng",
            html2: "R<span class='colorLetraRojo'>a</span>ng",
            html3: "R<span class='colorLetraRojo'>u</span>ng",
            d: "Tocar.",
          },
          {
            html1: "Shr<span class='colorLetraRojo'>i</span>nk",
            html2: "Shr<span class='colorLetraRojo'>a</span>nk",
            html3: "Shr<span class='colorLetraRojo'>u</span>nk",
            d: "Encoger.",
          },
          {
            html1: "S<span class='colorLetraRojo'>i</span>nk",
            html2: "S<span class='colorLetraRojo'>a</span>nk",
            html3: "S<span class='colorLetraRojo'>u</span>nk",
            d: "Hundir.",
          },
          {
            html1: "St<span class='colorLetraRojo'>i</span>nk",
            html2: "St<span class='colorLetraRojo'>a</span>nk",
            html3: "St<span class='colorLetraRojo'>u</span>nk",
            d: "Apestar.",
          },
          {
            html1: "Dr<span class='colorLetraRojo'>i</span>nk",
            html2: "Dr<span class='colorLetraRojo'>a</span>nk",
            html3: "Dr<span class='colorLetraRojo'>u</span>nk",
            d: "Beber.",
          },
        ],
      },
      tabla1P12: {
        fields: [
          { key: "a", label: "Present", thClass: "colorLetraRojo" },
          { key: "b", label: "Past", thClass: "colorLetraRojo" },
          { key: "c", label: "Participle ", thClass: "colorLetraRojo" },
          { key: "d", label: "Translation ", thClass: "colorLetraRojo" },
        ],
        items: [
          { a: "Tell", b: "Told", c: "Told", d: "Contar." },
          { a: "Say", b: "Said", c: "Said", d: "Decir." },
          { a: "Understand", b: "Understood", c: "Understood", d: "Entender." },
          { a: "Bleed", b: "Bled", c: "Bled", d: "Sangrar." },
          { a: "Bend", b: "Bent", c: "Bent", d: "Doblar." },
          { a: "Send", b: "Sent", c: "Sent", d: "Enviar." },
          { a: "Lend", b: "Lent", c: "Lent", d: "Prestar." },
          { a: "Light", b: "Lit", c: "Lit", d: "Encender." },
          { a: "Pay", b: "Paid", c: "Paid", d: "Pagar." },
          { a: "Breed", b: "Bred", c: "Bred", d: "Criar o reproducir." },
          { a: "Mean", b: "Meant", c: "Meant", d: "Querer decir." },
          { a: "Build", b: "Built", c: "Built", d: "Construir." },
          { a: "Cling", b: "Clung", c: "Clung", d: "Aferrarse." },
          { a: "Creep", b: "Crept", c: "Crept", d: "Trepar." },
          { a: "Deal", b: "Dealt", c: "Dealt", d: "Repartir." },
          { a: "Feed", b: "Fed", c: "Fed", d: "Alimentar." },
          { a: "Feel", b: "Felt", c: "Felt", d: "Sentir." },
          { a: "Find", b: "Found", c: "Found", d: "Encontrar." },
          { a: "Grind", b: "Ground", c: "Ground", d: "Moler." },
          { a: "Hear", b: "Heard", c: "Heard", d: "Oír." },
          { a: "Hold", b: "Held", c: "Held", d: "Sostener." },
          { a: "Keep", b: "Kept", c: "Kept", d: "Mantener." },
          { a: "Kneel", b: "Knelt", c: "Knelt", d: "Arrodillar." },
          { a: "Lay", b: "Laid", c: "Laid", d: "Poner." },
          { a: "Lead", b: "Led", c: "Led", d: "Dirigir." },
          { a: "Leave", b: "Left", c: "Left", d: "Dejar." },
          { a: "Lose", b: "Lost", c: "Lost", d: "Perder." },
          { a: "Make", b: "Made", c: "Made", d: "Hacer." },
          { a: "Meet", b: "Met", c: "Met", d: "Conocer." },
          { a: "Sell", b: "Sold", c: "Sold", d: "Vender." },
          { a: "Shoot", b: "Shot", c: "Shot", d: "Disparar." },
          { a: "Shine", b: "Shone", c: "Shone", d: "Alumbrar." },
          { a: "Sit", b: "Sat", c: "Sat", d: "Sentarse." },
          { a: "Sleep", b: "Slept", c: "Slept", d: "Dormir." },
          { a: "Slide", b: "Slid", c: "Slid", d: "Deslizar." },
          { a: "Spend", b: "Spent", c: "Spent", d: "Gastar." },
          { a: "Spit", b: "Spat", c: "Spat", d: "Escupir." },
          { a: "Stand", b: "Stood", c: "Stood", d: "Pararse." },
          { a: "Stick", b: "Stuck", c: "Stuck", d: "Pegar." },
          { a: "Sting", b: "Stung", c: "Stung", d: "Picar." },
          { a: "Strike", b: "Struck", c: "Struck", d: "Golpear." },
          { a: "Sweep", b: "Swept", c: "Swept", d: "Barrer." },
          { a: "Swing", b: "Swung", c: "Swung", d: "Balancearse." },
          { a: "Weep", b: "Wept", c: "Wept", d: "Llorar." },
          { a: "Win", b: "Won", c: "Won", d: "Ganar." },
          { a: "Wind", b: "Wound", c: "Wound", d: "Enrollar." },
          { a: "Have", b: "Had", c: "Had", d: "Tener." },
          { a: "Bind", b: "Bound", c: "Bound", d: "Amarrar." },
        ],
      },
      tabla2P11: {
        fields: [
          { key: "a", label: "Present", thClass: "colorLetraRojo" },
          { key: "b", label: "Past", thClass: "colorLetraRojo" },
          { key: "html2", label: "Participle ", thClass: "colorLetraRojo" },
          { key: "d", label: "Translation ", thClass: "colorLetraRojo" },
        ],
        items: [
          {
            a: "Hide",
            b: "Hid",
            d: "Esconder, esconderse",
            html2:
              "<span class='colorLetraAzul'>Hidd<span class='colorLetraRojo'>en",
          },
          {
            a: "Bite",
            b: "Bit",
            d: "Morder.",
            html2:
              "<span class='colorLetraAzul'>Bitt<span class='colorLetraRojo'>en",
          },
          {
            a: "Drive",
            b: "Drove",
            d: "Conducir.",
            html2:
              "<span class='colorLetraAzul'>Driv<span class='colorLetraRojo'>en",
          },
          {
            a: "Write",
            b: "Wrote",
            d: "Escribir.",
            html2:
              "<span class='colorLetraAzul'>Writt<span class='colorLetraRojo'>en",
          },
          {
            a: "Ride",
            b: "Rode",
            d: "Subir.",
            html2:
              "<span class='colorLetraAzul'>Rid<span class='colorLetraRojo'>en",
          },
          {
            a: "Rise",
            b: "Rose",
            d: "Montar.",
            html2:
              "<span class='colorLetraAzul'>Ris<span class='colorLetraRojo'>en",
          },
          {
            a: "Take",
            b: "Took",
            d: "Llevar o tomar.",
            html2:
              "<span class='colorLetraAzul'>Tak<span class='colorLetraRojo'>en",
          },
          {
            a: "See",
            b: "Saw",
            d: "Ver.",
            html2:
              "<span class='colorLetraAzul'>Se<span class='colorLetraRojo'>en",
          },
          {
            a: "Eat",
            b: "Ate",
            d: "Comer.",
            html2:
              "<span class='colorLetraAzul'>Eat<span class='colorLetraRojo'>en",
          },
          {
            a: "Wake",
            b: "Woke",
            d: "Despertar.",
            html2:
              "<span class='colorLetraAzul'>Wok<span class='colorLetraRojo'>en",
          },
          {
            a: "Speak",
            b: "Spoke",
            d: "Hablar.",
            html2:
              "<span class='colorLetraAzul'>Spok<span class='colorLetraRojo'>en",
          },
          {
            a: "Break",
            b: "Broke",
            d: "Romper.",
            html2:
              "<span class='colorLetraAzul'>Brok<span class='colorLetraRojo'>en",
          },
          {
            a: "Freeze",
            b: "Froze",
            d: "Congelar.",
            html2:
              "<span class='colorLetraAzul'>Froz<span class='colorLetraRojo'>en",
          },
          {
            a: "Shake",
            b: "Shook",
            d: "Sacudir.",
            html2:
              "<span class='colorLetraAzul'>Shak<span class='colorLetraRojo'>en",
          },
          {
            a: "Forget",
            b: "Forgot",
            d: "Olvidar.",
            html2:
              "<span class='colorLetraAzul'>Forgott<span class='colorLetraRojo'>en",
          },
          {
            a: "Steal",
            b: "Stole",
            d: "Robar.",
            html2:
              "<span class='colorLetraAzul'>Stol<span class='colorLetraRojo'>en",
          },
          {
            a: "Choose",
            b: "Chose",
            d: "Elegir.",
            html2:
              "<span class='colorLetraAzul'>Chos<span class='colorLetraRojo'>en",
          },
          {
            a: "Give",
            b: "Gave",
            d: "Dar.",
            html2:
              "<span class='colorLetraAzul'>Giv<span class='colorLetraRojo'>en",
          },
          {
            a: "Forgive",
            b: "Forgave",
            d: "Olvidar.",
            html2:
              "<span class='colorLetraAzul'>Forgiv<span class='colorLetraRojo'>en",
          },
          {
            a: "Forbid",
            b: "Forbade",
            d: "Prohibir.",
            html2:
              "<span class='colorLetraAzul'>Forbidd<span class='colorLetraRojo'>en",
          },
          {
            a: "Fall",
            b: "Fell",
            d: "Caer.",
            html2:
              "<span class='colorLetraAzul'>Fall<span class='colorLetraRojo'>en",
          },
        ],
      },
      tabla1P11: {
        fields: [
          { key: "a", label: "Present", thClass: "colorLetraRojo" },
          { key: "html1", label: "Past", thClass: "colorLetraRojo" },
          { key: "html2", label: "Participle ", thClass: "colorLetraRojo" },
          { key: "d", label: "Translation ", thClass: "colorLetraRojo" },
        ],
        items: [
          {
            a: "Buy",
            html1: "Bou<span class='colorLetraRojo'>ght",
            html2: "Bou<span class='colorLetraRojo'>ght",
            d: "Comprar.",
          },
          {
            a: "Think",
            html1: "Thou<span class='colorLetraRojo'>ght",
            html2: "Thou<span class='colorLetraRojo'>ght",
            d: "Pensar.",
          },
          {
            a: "Catch",
            html1: "Cau<span class='colorLetraRojo'>ght",
            html2: "Cau<span class='colorLetraRojo'>ght",
            d: "Atrapar.",
          },
          {
            a: "Teach",
            html1: "Tau<span class='colorLetraRojo'>ght",
            html2: "Tau<span class='colorLetraRojo'>ght",
            d: "Enseñar.",
          },
          {
            a: "Bring",
            html1: "Brou<span class='colorLetraRojo'>ght",
            html2: "Brou<span class='colorLetraRojo'>ght",
            d: "Traer.",
          },
          {
            a: "Fight",
            html1: "Fou<span class='colorLetraRojo'>ght",
            html2: "Fou<span class='colorLetraRojo'>ght",
            d: "Pelear.",
          },
        ],
      },
      tabla1P10: {
        fields: [
          { key: "a", label: "Present", thClass: "colorLetraRojo" },
          { key: "b", label: "Past", thClass: "colorLetraRojo" },
          { key: "c", label: "Participle ", thClass: "colorLetraRojo" },
          { key: "d", label: "Translation ", thClass: "colorLetraRojo" },
        ],
        items: [
          {
            a: "Set",
            b: "Set",
            c: "Set",
            d: "Configurar, ajustar, programar, organizar.",
          },
          { a: "Let", b: "Let", c: "Let", d: "Permitir, dejar." },
          { a: "Cut", b: "Cut", c: "Cut", d: "Cortar." },
          { a: "Put", b: "Put", c: "Put", d: "Poner." },
          { a: "Hit", b: "Hit", c: "Hit", d: "Golpear." },
          { a: "Hurt", b: "Hurt", c: "Hurt", d: "Lastimar." },
          { a: "Broadcast", b: "Broadcast", c: "Broadcast", d: "Transmitir." },
          { a: "Bet", b: "Bet", c: "Bet", d: "Apostar." },
          { a: "Shut", b: "Shut", c: "Shut", d: "Cerrar." },
          { a: "Read", b: "Read", c: "Read", d: "Leer." },
          { a: "Spread", b: "Spread", c: "Spread", d: "Extender." },
          { a: "Quit", b: "Quit", c: "Quit", d: "Renunciar a." },
          { a: "Burst", b: "Burst", c: "Burst", d: "Estallar." },
          { a: "Cost", b: "Cost", c: "Cost", d: "Costar." },
          { a: "Shed", b: "Shed", c: "Shed", d: "Perder la piel." },
        ],
      },
    };
  },
};
</script>

<style scoped>
</style>