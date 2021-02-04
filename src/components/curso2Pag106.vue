<template>
  <div>
    <b-container fluid>
      <b-row>
        <b-col></b-col>
        <b-col sm="auto">
          <h3 class="titulo">SUFFIXES “ER AND EST”</h3>
        </b-col>
        <b-col></b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i> </b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">Ambas sufijos significan <b>“más”</b></h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"> </b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            <b>ER:</b> se agrega al final del adjetivo y se usa con la palabra
            <b>“than”</b> que significa <b>“que”</b>
          </h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="7">
          <tablaTC :cuestionario="tabla3P7" />
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"> </b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            <b>EST:</b> se le agrega al final del adjetivo, pero debe ir antes
            la palabra <b>“the”</b> que significa <b>“el, la, lo, las, los”.</b>
          </h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="7">
          <tablaTC :cuestionario="tabla4P7" />
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"> </b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            Si el adjetivo es de tres silabas o más se usa <b>“MORE”</b> o
            <b>“THE MOST”</b> en lugar de
            <b
              >“ER-EST” <br />
              MORE.........(THAN)</b
            >
          </h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="7">
          <tablaTC :cuestionario="tabla5P7" />
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="11">
          <h3 class="subTitulo">
            THE MOST
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="7">
          <tablaTC :cuestionario="tabla6P7" />
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="11">
          <h3 class="subTitulo">
            RULES TO ADD THE ER AND EST
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"> </b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            <b>1.</b> Si el adjetivo es de una sílaba doblamos la última
            consonante y agregamos <b>ER.</b>
          </h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="7">
          <tablaTC :cuestionario="tabla7P7" />
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"> </b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            <b>2.</b> Si el adjetivo tiene dos silabas y termina en
            <b>“Y”</b> se cambia por <b>I</b> y se le agrega <b>ER.</b>
          </h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="7">
          <tablaTC :cuestionario="tabla8P7" />
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i> </b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">Write the english translation</h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="8">
          <tablaTC :cuestionario="tabla9P7" />
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="11">
          <h3 class="subTitulo">
            EXCEPCIONES DEL ER Y EST
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i> </b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            Estás palabras son adjetivos irregulares que no cumplen la regla del
            <b>er</b> o <b>est.</b>
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="9">
          <tablaTC :cuestionario="tabla10P7" />
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="11">
          <h3 class="subTitulo">
            LET´S PRACTICE
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3>
            <b>1.</b> Today is the best day of my life <br /><br />
            <b>2.</b> It could have been worse <br /><br />
            <b>3.</b> You can do it better next time <br /><br />
            <b>4.</b> You can get further if you wish <br /><br />
            <b>5.</b> That is the worst mistake I have ever made <br /><br />
            <b>6.</b> This is good, but It could be better <br /><br />
            <b>7.</b> I have walked the further today <br /><br />
            <b>8.</b> This place looks better than last night <br /><br />
            <b>9.</b> Excuse me, do you have a bigger plastic bag than this one?
            <br /><br />
            <b>10.</b> When I was younger I could run faster than now
            <br /><br />
            <b>11.</b> Learning English is easier than I thought <br /><br />
            <b>12.</b> I feel the happiest person in the world.
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="11">
          <h3 class="subTitulo">
            OTRAS FORMAS DE COMPARAR
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i> </b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            <span class="colorLetraRojo">AS</span>_______
            <span class="colorLetraRojo">AS</span>(el primer
            <b>“AS”</b> significa <b>“TAN”</b> y el segundo significa
            <b>“COMO”</b>)
          </h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3>
            <b>1.</b> Today is <span class="colorLetraRojo">as</span> hot
            <span class="colorLetraRojo">as</span> yesterday: hoy es tan
            caliente como ayer <br /><br />
            <b>2.</b> She is not <span class="colorLetraRojo">as</span> bad
            <span class="colorLetraRojo">as</span> everybody says: ella no es
            tan mala como todo el mundo dice.
          </h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i> </b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            <span class="colorLetraRojo">LESS THAN</span> (menos que, menos de,
            a menos de, inferior a)
          </h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3>
            <b>1.</b> I have <b>less</b> money than yesterday: tengo menos
            dinero que ayer <br /><br />
            <b>2.</b> The bus has left <b>less</b> than a minute ago: el bus se
            fue hace menos de un minuto
          </h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i> </b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            <span class="colorLetraRojo">THE SAME</span>___
            <span class="colorLetraRojo">AS</span> (lo mismo que)
          </h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3>
            <b>1.</b> Are you the <span class="colorLetraRojo">same</span> age
            <span class="colorLetraRojo">as</span> me? ¿Tienes la misma edad que
            yo? <br /><br />
            <b>2.</b> Your eyes are the
            <span class="colorLetraRojo">same</span> colour
            <span class="colorLetraRojo">as</span> mine.
          </h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i> </b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            Filing in the gaps with AS….AS, MORE, ER, THAN
          </h3>
        </b-col>
      </b-row>
      <br>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            <b>1.</b> Tú eres tan terco como una mula. You are 
          </h3>
        </b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['as']"
            tamano="7"
          />
        </b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            stubborn 
          </h3>
        </b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['as']"
            tamano="7"
          />
        </b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            a mule. 
          </h3>
        </b-col>
      </b-row>
      <br>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            <b>2.</b> Te amo más que nunca. I love you 
          </h3>
        </b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['more']"
            tamano="8"
          />
        </b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            than ever.
          </h3>
        </b-col>
      </b-row>
      <br>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            <b>3.</b>	No creo que este carro sea más costoso que aquel. I don´t think that car is 
          </h3>
        </b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['more']"
            tamano="8"
          />
        </b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            expensive 
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['than']"
            tamano="7.5"
          />
        </b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            that one. 
          </h3>
        </b-col>
      </b-row>
      <br>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            <b>4.</b> Esta casa es más grande que ese castillo. This house is 
          </h3>
        </b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['bigger']"
            tamano="9.5"
          />
        </b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            (Big)than that castle.
          </h3>
        </b-col>
      </b-row>
      <br>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            <b>5.</b>	me levante más tarde que ayer. This morning I got up 
          </h3>
        </b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['later']"
            tamano="8"
          />
        </b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            (Late) than yesterday.
          </h3>
        </b-col>
      </b-row>
      <br>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            <b>6.</b>	Esto es más fácil de lo que yo pensé.  This is 
          </h3>
        </b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['easier']"
            tamano="10"
          />
        </b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            (easy)
          </h3>
        </b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['than']"
            tamano="8"
          />
        </b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            I thought.
          </h3>
        </b-col>
      </b-row>
      <br>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            <b>7.</b>	Quédate un poco más de tiempo. Stay for a Little bit 
          </h3>
        </b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['longer']"
            tamano="9"
          />
        </b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            (long).
          </h3>
        </b-col>
      </b-row>
      <br>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            <b>8.</b> Entre más rápido, mejor. The 
          </h3>
        </b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['faster']"
            tamano="9"
          />
        </b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            (fast), the better. 
          </h3>
        </b-col>
      </b-row>
      <br>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            <b>9.</b> Hay menos manzanas que ayer. There are  
          </h3>
        </b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['fewwer']"
            tamano="9"
          />
        </b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            (few) apples than yesterday.
          </h3>
        </b-col>
      </b-row>
      <br>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            <b>10.</b>	Tú eres de la misma edad que yo. You are the 
          </h3>
        </b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['same']"
            tamano="8"
          />
        </b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            age
          </h3>
        </b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['than']"
            tamano="8"
          />
        </b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            me.
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="11">
          <h3 class="subTitulo">
            LOGIC TABLES
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="7">
          <tablaTC :cuestionario="tabla11P7" />
        </b-col>
      </b-row>
      <br>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="10">
          <tablaTC :cuestionario="tabla12P7" />
        </b-col>
      </b-row>
      <br>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="7">
          <tablaTC :cuestionario="tabla13P7" />
        </b-col>
      </b-row>
      <br>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="10">
          <tablaTC :cuestionario="tabla14P7" />
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
      tabla3P7: {
        fields: [
          { key: "a", thClass: "noHead" },
          { key: "html1", thClass: "noHead" },
          { key: "html2", thClass: "noHead" },
        ],
        items: [
          {
            a: "Big",
            html1: "Bigg<span class='colorLetraRojo'>er than</span>",
            html2: "<span class='colorLetraRojo'>Más</span> grande que",
          },
          {
            a: "Small",
            html1: "Small<span class='colorLetraRojo'>er than</span>",
            html2: "<span class='colorLetraRojo'>Más</span> pequeño que",
          },
        ],
      },
      tabla4P7: {
        fields: [
          { key: "a", thClass: "noHead" },
          { key: "html1", thClass: "noHead" },
          { key: "html2", thClass: "noHead" },
        ],
        items: [
          {
            a: "Big",
            html1: "The Bigg<span class='colorLetraRojo'>est</span>",
            html2: "<span class='colorLetraRojo'>El más</span> grande",
          },
          {
            a: "Small",
            html1: "The Small<span class='colorLetraRojo'>est</span>",
            html2: "<span class='colorLetraRojo'>El más</span> pequeño",
          },
        ],
      },
      tabla5P7: {
        fields: [
          { key: "a", thClass: "noHead" },
          { key: "html1", thClass: "noHead" },
          { key: "html2", thClass: "noHead" },
        ],
        items: [
          {
            a: "Expensive",
            html1:
              "<span class='colorLetraRojo'>More</span> expensive <span class='colorLetraRojo'>than</span>",
            html2: "<span class='colorLetraRojo'>Más</span> costoso que",
          },
          {
            a: "Beautiful",
            html1:
              "<span class='colorLetraRojo'>More</span> beautiful <span class='colorLetraRojo'>than</span>",
            html2: "<span class='colorLetraRojo'>Más</span> hermoso que",
          },
        ],
      },
      tabla6P7: {
        fields: [
          { key: "a", thClass: "noHead" },
          { key: "html1", thClass: "noHead" },
          { key: "html2", thClass: "noHead" },
        ],
        items: [
          {
            a: "Interesting",
            html1: "<span class='colorLetraRojo'>The most</span> interesting",
            html2: "<span class='colorLetraRojo'>El más</span> interesante",
          },
          {
            a: "comfortable",
            html1: "<span class='colorLetraRojo'>The most</span> comfortable",
            html2: "<span class='colorLetraRojo'>El más</span> comodo",
          },
        ],
      },
      tabla7P7: {
        fields: [
          { key: "a", thClass: "noHead" },
          { key: "b", thClass: "noHead" },
          { key: "html1", thClass: "noHead" },
          { key: "html2", thClass: "noHead" },
        ],
        items: [
          {
            a: "Caliente",
            b: "Hot",
            html1: "Ho<span class='colorLetraRojo'>tter</span>",
            html2: "The hot<span class='colorLetraRojo'>test</span>",
          },
          {
            a: "Grande",
            b: "Big",
            html1: "Bi<span class='colorLetraRojo'>gger</span>",
            html2: "The big<span class='colorLetraRojo'>gest</span>",
          },
          {
            a: "Gordo",
            b: "Fat",
            html1: "Fat<span class='colorLetraRojo'>ter</span>",
            html2: "The fat<span class='colorLetraRojo'>test</span>",
          },
        ],
      },
      tabla8P7: {
        fields: [
          { key: "a", thClass: "noHead" },
          { key: "html3", thClass: "noHead" },
          { key: "html1", thClass: "noHead" },
          { key: "html2", thClass: "noHead" },
        ],
        items: [
          {
            a: "Feliz",
            html3: "Happ<span class='colorLetraRojo'>y</span>",
            html1: "Happ<span class='colorLetraRojo'>ier</span>",
            html2: "The happ<span class='colorLetraRojo'>iest</span>",
          },
          {
            a: "Fácil",
            html3: "Eas<span class='colorLetraRojo'>y</span>",
            html1: "Eas<span class='colorLetraRojo'>ier</span>",
            html2: "The eas<span class='colorLetraRojo'>iest</span>",
          },
          {
            a: "Exigente",
            html3: "Pick<span class='colorLetraRojo'>y</span>",
            html1: "Pick<span class='colorLetraRojo'>ier</span>",
            html2: "The pick<span class='colorLetraRojo'>iest</span>",
          },
        ],
      },
      tabla9P7: {
        fields: [
          { key: "a", thClass: "noHead" },
          { key: "b", thClass: "noHead" },
          { key: "c", thClass: "noHead" },
          { key: "complejo1", thClass: "noHead" },
        ],
        items: [
          {
            a: "Divertido",
            b: "Funny",
            c: "El más divertido",
            complejo1: {
              lista: ["The funniest"],
              tamano: 12.5,
              resuelto: false,
            },
          },
          {
            a: "Feliz",
            b: "Happy",
            c: "Más feliz que",
            complejo1: { lista: ["Happier than"], tamano: 13, resuelto: false },
          },
          {
            a: "Angosto",
            b: "Narrow",
            c: "El más angosto ",
            complejo1: {
              lista: ["The narrowest"],
              tamano: 14,
              resuelto: false,
            },
          },
          {
            a: "Valioso",
            b: "Valuable",
            c: "Más valioso que",
            complejo1: {
              lista: ["More valuable than"],
              tamano: 17,
              resuelto: false,
            },
          },
          {
            a: "Oscuro",
            b: "Dark",
            c: "El más oscuro",
            complejo1: {
              lista: ["The darkest"],
              tamano: 12.5,
              resuelto: false,
            },
          },
          {
            a: "Feliz",
            b: "Happy",
            c: "El más feliz",
            complejo1: {
              lista: ["The happier"],
              tamano: 12.5,
              resuelto: false,
            },
          },
          {
            a: "Caliente",
            b: "Hot",
            c: "Más caliente que",
            complejo1: {
              lista: ["Hotter than"],
              tamano: 12.5,
              resuelto: false,
            },
          },
          {
            a: "Grande",
            b: "Big",
            c: "El más grande",
            complejo1: {
              lista: ["The biggest"],
              tamano: 12.5,
              resuelto: false,
            },
          },
          {
            a: "Delgado",
            b: "Thin",
            c: "Más delgado que",
            complejo1: {
              lista: ["Thiner than"],
              tamano: 12.5,
              resuelto: false,
            },
          },
          {
            a: "Delgado",
            b: "Thin",
            c: "El más delgado",
            complejo1: {
              lista: ["The thinnest"],
              tamano: 12.5,
              resuelto: false,
            },
          },
          {
            a: "Duro",
            b: "Hard",
            c: "Más duro que",
            complejo1: {
              lista: ["Harder than"],
              tamano: 12.5,
              resuelto: false,
            },
          },
          {
            a: "Difícil",
            b: "Difficult",
            c: "Más difícil que",
            complejo1: {
              lista: ["More difficult than"],
              tamano: 16,
              resuelto: false,
            },
          },
          {
            a: "Viejo",
            b: "Old",
            c: "Más viejo que",
            complejo1: { lista: ["Older than"], tamano: 12.5, resuelto: false },
          },
          {
            a: "Fácil",
            b: "Easy",
            c: "El más fácil",
            complejo1: {
              lista: ["The easiest"],
              tamano: 12.5,
              resuelto: false,
            },
          },
        ],
      },
      tabla10P7: {
        fields: [
          { key: "a", label: "" },
          { key: "b", label: "" },
          { key: "c", label: "ER" },
          { key: "d", label: "" },
          { key: "e", label: "EST" },
          { key: "f", label: "" },
        ],
        items: [
          {
            a: "Bueno",
            b: "Good",
            c: "Better",
            d: "Mejor",
            e: "The best",
            f: "El mejor",
          },
          {
            a: "Malo",
            b: "Bad",
            c: "Worse",
            d: "Peor",
            e: "The worst",
            f: "El peor",
          },
          {
            a: "Far",
            b: "Lejos",
            c: "Further",
            d: "Mas lejos",
            e: "The furthest/ farthest",
            f: "El más lejos",
          },
        ],
      },
      tabla11P7: {
        fields: [
          { key: "a", thClass:"noHead" },
          { key: "b", thClass:"noHead" },
          { key: "c", thClass:"noHead" },
        ],
        items: [
          {
            a: "1.she is",
            b: "1.Better than",
            c: "1.me",
          },
          {
            a: "2.You are",
            b: "2.More beautiful than",
            c: "2.her",
          },
          {
            a: "3.We are",
            b: "3.Faster than",
            c: "3.Him",
          },
          {
            a: "4.My life is",
            b: "4.Sadder than",
            c: "4.Us",
          },
          {
            a: "5.This house is",
            b: "5.Bigger than",
            c: "5.Them",
          },
          {
            a: "6.My car is",
            b: "6.As interesting as",
            c: "6.Yours",
          },
          {
            a: "7.I am",
            b: "7.Less expensive than",
            c: "7.You",
          },
        ],
      },
      tabla12P7: {
        fields: [
          { key: "a", thClass:"noHead" },
          { key: "b", thClass:"noHead" },
          { key: "c", thClass:"noHead" },
          { key: "complejo1", label:"ENGLISH" },
          { key: "complejo2", label:"SPANISH"}
        ],
        items: [
          {
            a: "1",
            b: "1",
            c: "1",
            complejo1: {lista: ["She is better tan me"],tamano: 18,resuelto: false,},
            complejo2: {lista: ["Ella es mejor que yo"],tamano: 18,resuelto: false,},
          },
          {
            a: "1",
            b: "2",
            c: "2",
            complejo1: {lista: ["She is more beautiful tan her"],tamano: 23,resuelto: false,},
            complejo2: {lista: ["Ella es más hermosa que ella"],tamano: 23,resuelto: false,},
          },
          {
            a: "1",
            b: "3",
            c: "1",
            complejo1: {lista: ["She is faster tan me"],tamano: 18,resuelto: false,},
            complejo2: {lista: ["Ella es más rapida que yo"],tamano: 21,resuelto: false,},
          },
          {
            a: "2",
            b: "6",
            c: "2",
            complejo1: {lista: ["You are as interesting as her"],tamano: 22.5,resuelto: false,},
            complejo2: {lista: ["Eres tan interesante como ella"],tamano: 23.5,resuelto: false,},
          },
          {
            a: "4",
            b: "4",
            c: "6",
            complejo1: {lista: ["My life is sadder tan yours"],tamano: 21.3,resuelto: false,},
            complejo2: {lista: ["Mi vida es más triste que la tuya"],tamano: 24.5,resuelto: false,},
          },
          {
            a: "5",
            b: "5",
            c: "6",
            complejo1: {lista: ["This house is bigger tan yours"],tamano: 23.5,resuelto: false,},
            complejo2: {lista: ["Esta casa es más grande que la tuya"],tamano: 27,resuelto: false,},
          },
          {
            a: "6",
            b: "7",
            c: "6",
            complejo1: {lista: ["My car is less expensive tan yours"],tamano: 26,resuelto: false,},
            complejo2: {lista: ["Mi carro es menos caro que el tuyo"],tamano: 26,resuelto: false,},
          },
          {
            a: "3",
            b: "3",
            c: "7",
            complejo1: {lista: ["We are faster tan you"],tamano: 18.4,resuelto: false,},
            complejo2: {lista: ["Nosotros somos más rapidos que tu"],tamano: 26.5,resuelto: false,},
          },
          {
            a: "5",
            b: "7",
            c: "6",
            complejo1: {lista: ["This house is less expensive than yours"],tamano: 28.5,resuelto: false,},
            complejo2: {lista: ["Esta casa es menos cara que la tuya"],tamano: 27,resuelto: false,},
          },
          {
            a: "7",
            b: "1",
            c: "7",
            complejo1: {lista: ["I am better than you"],tamano: 18,resuelto: false,},
            complejo2: {lista: ["Yo soy mejor que tú"],tamano: 17.5,resuelto: false,},
          },
          {
            a: "7",
            b: "6",
            c: "5",
            complejo1: {lista: ["I am as interesting as them"],tamano: 22,resuelto: false,},
            complejo2: {lista: ["Yo soy tan interesante como ellos"],tamano: 26,resuelto: false,},
          },
        ],
      },
      tabla13P7: {
        fields: [
          { key: "a", thClass:"noHead" },
          { key: "b", thClass:"noHead" },
          { key: "c", thClass:"noHead" },
        ],
        items: [
          {
            a: "1.She is",
            b: "1.The best friend",
            c: "1.Of all",
          },
          {
            a: "2.You are",
            b: "2.The most beautiful woman",
            c: "2.In the world",
          },
          {
            a: "3.We are",
            b: "3.The fastest runner/runners",
            c: "3.Runner",
          },
          {
            a: "4.My life is",
            b: "4.The funniest story",
            c: "4.Story",
          },
          {
            a: "5.This house is",
            b: "5.The biggest",
            c: "5.I have ever had",
          },
          {
            a: "6.This car is",
            b: "6.The worst",
            c: "6.I have ever seen",
          },
          {
            a: "7.I have",
            b: "7.The oldest",
            c: "",
          },
        ],
      },
      tabla14P7: {
        fields: [
          { key: "a", thClass:"noHead" },
          { key: "b", thClass:"noHead" },
          { key: "c", thClass:"noHead" },
          { key: "complejo1", label:"ENGLISH" },
          { key: "complejo2", label:"SPANISH"}
        ],
        items: [
          {
            a: "1",
            b: "1",
            c: "1",
            complejo1: {lista: ["She is the best friend of all"],tamano: 21,resuelto: false,},
            complejo2: {lista: ["Ella es la mejor amiga de todas"],tamano: 23.5,resuelto: false,},
          },
          {
            a: "1",
            b: "2",
            c: "2",
            complejo1: {lista: ["She is the most beautiful in the world"],tamano: 26.7,resuelto: false,},
            complejo2: {lista: ["Ella es la más linda del mundo"],tamano: 23,resuelto: false,},
          },
          {
            a: "1",
            b: "3",
            c: "1",
            complejo1: {lista: ["She is the fastest runner in the world"],tamano: 27,resuelto: false,},
            complejo2: {lista: ["Ella es la corredora más rápida del mundo"],tamano: 30,resuelto: false,},
          },
          {
            a: "2",
            b: "6",
            c: "3",
            complejo1: {lista: ["You are the worst runner"],tamano: 20,resuelto: false,},
            complejo2: {lista: ["Tu eres el peor corredor"],tamano: 20,resuelto: false,},
          },
          {
            a: "4",
            b: "4",
            c: "2",
            complejo1: {lista: ["My life is the funniest in the world"],tamano: 25,resuelto: false,},
            complejo2: {lista: ["Mi vida es la más divertida del mundo"],tamano: 27.3,resuelto: false,},
          },
          {
            a: "5",
            b: "5",
            c: "6",
            complejo1: {lista: ["This house is the biggest i have ever seen"],tamano: 30,resuelto: false,},
            complejo2: {lista: ["Esta casa es la más grande que he visto"],tamano: 29,resuelto: false,},
          },
          {
            a: "6",
            b: "7",
            c: "3",
            complejo1: {lista: ["This car is the oldest runner"],tamano: 22,resuelto: false,},
            complejo2: {lista: ["Este auto es el corredor más viejo"],tamano: 26,resuelto: false,},
          },
          {
            a: "3",
            b: "3",
            c: "2",
            complejo1: {lista: ["We are the fastest runners in the world"],tamano: 28,resuelto: false,},
            complejo2: {lista: ["Nosotros somos los corredores más rápidos del mundo"],tamano: 37.3,resuelto: false,},
          },
        ],
      },
    };
  },
};
</script>
