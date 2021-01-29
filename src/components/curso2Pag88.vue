<template>
  <div>
    <b-container fluid>
      <b-row>
        <b-col></b-col>
        <b-col sm="auto">
          <h3 class="titulo">A GREAT STORY</h3>
        </b-col>
        <b-col></b-col>
      </b-row>

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
            THIS READING IS ABOUT THE BEGINNING OF AMERICAN LAND
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            In 2006, the director of American Land decided to join the Colombian
            Army, when he was 21 years old. After a few days in the military he
            was chosen among several soldiers at the presidential guard
            battalion in Bogotá. In early January 2007 he flew to Cairo to work
            for the M.F.O. (Multinational Force and Observers). The
            Multinational Force & Observers (MFO), headquartered in Rome, is an
            independent, international organization, created by agreement
            between the Arab Republic of Egypt and the State of Israel, with
            peacekeeping responsibilities in the Sinai peninsula.
            <br /><br />
            At the base there were twelve bars, including ́ ́Colombian Land ́ ́,
            which translates to ́ ́Tierra Colombiana ́ in Spanish. On Thursdays
            Colombian soldiers would go there to enjoy the company of their
            friends and other soldiers.
            <br /><br />
            Most Colombian soldiers did ́t speak English and felt frustrated by
            not being able to communicate with the other soldiers from different
            countries, whereas the English-Spanish interpreters could speak with
            anyone on the base.
            <br /><br />
            After retúrning to Colombia the founder of American Land settled
            down in Pitalito, where his younger brother lived.
            <span class="colorLetraRojo">
              One day he stopped by a place to hand some documents over to
              someone and on his way out he</span
            >
            saw a sign that read “English Classes”, so he asked for further
            information as he was very interested in teaching English. He was
            hired that very day to teach kids the next morning. A year later, he
            decided to open his own English academy in Pitalito. <br /><br />
            His dream hadfinally come into fruition –he first named the
            institútion “Colombian Land”, as a homage to the bar on base, and
            later renamed it “American Land”. Slowly but surely, “American Land”
            began to grow in the number of stúdents and reputation, with much
            help from then 17-year-old Seth Goodrow.
          </h3>
        </b-col>
        <b-col sm="1"></b-col>
      </b-row>

      <br /><br />

      <b-row>
        <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            Fill in the gaps with the following words:
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            <b>
              Join - decided - few - chosen - several - early - flew -
              headquarted - agreement - peacekeeping - there are - enjoy -
              frustrated - whereas - anyone - retúrning - director - settled
              down - hand - over - sign as - hired - teach - decided - own -
              fruition - homage - reputation.
            </b>
          </h3>
        </b-col>
        <b-col sm="1"></b-col>
      </b-row>

      <br />
      <b-row>
        <b-col sm="auto"></b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">
            In 2006, the director of American Land
          </h3>
        </b-col>

        <b-col sm="left">
          <inputChecked :resuelto="false" :esperado="['decided']" tamano="12" />
        </b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">to</h3>
        </b-col>

        <b-col sm="left">
          <inputChecked :resuelto="false" :esperado="['join']" tamano="9.3" />
        </b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">
            the Colombian Army, when he was
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">
            21 years old. After a
          </h3>
        </b-col>

        <b-col sm="left">
          <inputChecked :resuelto="false" :esperado="['few']" tamano="9.3" />
        </b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">days in the military he was</h3>
        </b-col>

        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['chosen']"
            tamano="11.3"
          />
        </b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">
            among
          </h3>
        </b-col>

        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['several']"
            tamano="11.5"
          />
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">
            soldiers at the presidential guard battalion in Bogotá. In
          </h3>
        </b-col>

        <b-col sm="left">
          <inputChecked :resuelto="false" :esperado="['early']" tamano="10" />
        </b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">January 2007 he</h3>
        </b-col>

        <b-col sm="left">
          <inputChecked :resuelto="false" :esperado="['flew']" tamano="10" />
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">
            to Cairo to work for the M.F.O. (Multinational Force and Observers).
            The Multinational Force & Observers (MFO),
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>

        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['headquartered']"
            tamano="16"
          />
        </b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">
            in Rome, is an independent international organization, created by
          </h3>
        </b-col>

        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['agreement']"
            tamano="14"
          />
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">
            between the Arab Republic of Egypt and the State of Israel, with
          </h3>
        </b-col>

        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['peacekeeping']"
            tamano="15.2"
          />
        </b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">responsibilities in the Sinai</h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">
            peninsula.
          </h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="auto"></b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">
            At the base
          </h3>
        </b-col>

        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['there are']"
            tamano="12.5"
          />
        </b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">
            twelve bars, including ´´Colombian Land´´, which translates to
            ´´Tierra Colombiana´´
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">
            in Spanish. On Thursdays Colombian soldiers go to the bar to
          </h3>
        </b-col>

        <b-col sm="left">
          <inputChecked :resuelto="false" :esperado="['enjoy']" tamano="10.3" />
        </b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">the company of their friends and other</h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">
            soldiers.
          </h3>
        </b-col>
      </b-row>

      <br />
      <b-row>
        <b-col sm="auto"></b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">
            Most Colombian soldiers didn´t speak English and felt
          </h3>
        </b-col>

        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['frustrated']"
            tamano="13"
          />
        </b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">by not being able to communicate</h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">
            with the other soldiers from different countries,
          </h3>
        </b-col>

        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['whereas']"
            tamano="12.5"
          />
        </b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">
            the English-Spanish interpreters could speak with
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>

        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['anyone']"
            tamano="12.5"
          />
        </b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">on the base.</h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="auto"></b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">
            After
          </h3>
        </b-col>

        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['returning']"
            tamano="12.5"
          />
        </b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">to Colombia the</h3>
        </b-col>

        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['director']"
            tamano="12"
          />
        </b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">of American Land</h3>
        </b-col>

        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['settled down']"
            tamano="15"
          />
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            in Pitalito, where his younger brother lived. One day he stopped by
            a place to
          </h3>
        </b-col>

        <b-col sm="left">
          <inputChecked :resuelto="false" :esperado="['hand']" tamano="10.5" />
        </b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">some documents</h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>

        <b-col sm="left">
          <inputChecked :resuelto="false" :esperado="['over']" tamano="10" />
        </b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">to someone and on his way out he saw a</h3>
        </b-col>

        <b-col sm="left">
          <inputChecked :resuelto="false" :esperado="['sign']" tamano="9.5" />
        </b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">
            that read “English Classes”, so he asked for
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">further information</h3>
        </b-col>

        <b-col sm="left">
          <inputChecked :resuelto="false" :esperado="['as']" tamano="9" />
        </b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">
            he was very interested in teaching English. He was
          </h3>
        </b-col>

        <b-col sm="left">
          <inputChecked :resuelto="false" :esperado="['hired']" tamano="11" />
        </b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">that very</h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">day to</h3>
        </b-col>

        <b-col sm="left">
          <inputChecked :resuelto="false" :esperado="['teach']" tamano="11" />
        </b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">kids the next morning. A year later, he</h3>
        </b-col>

        <b-col sm="left">
          <inputChecked :resuelto="false" :esperado="['decided']" tamano="11" />
        </b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">to open his</h3>
        </b-col>

        <b-col sm="left">
          <inputChecked :resuelto="false" :esperado="['own']" tamano="9.5" />
        </b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">English</h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">institúte in Pitalito.</h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="auto"></b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">His dream had finally come into</h3>
        </b-col>

        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['fruition']"
            tamano="11"
          />
        </b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">
            - he first named the institútion “Colombian Land”, as a
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>

        <b-col sm="left">
          <inputChecked :resuelto="false" :esperado="['homage']" tamano="12" />
        </b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">
            to the bar on base, and later renamed it “American Land”. Slowly but
            surely, “American Land” began
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">to grow in number of students and</h3>
        </b-col>

        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['reputation']"
            tamano="13"
          />
        </b-col>

        <b-col sm="auto">
          <h3 class="parrafoIC">
            , with much help from then 17-year-old Seth Goodrow.
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="11">
          <h3 class="subTitulo">COMPREHENSION:</h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            <b>Q1. </b>How old was the director of American Land when he joined
            the army? What year was it?
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <inputChecked
            :resuelto="false"
            :esperado="['The year was 2006 and he was 21 years old']"
            tamano="33"
          />
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            <b>Q2. </b>What was the original name of American Land? Why?
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <inputChecked
            :resuelto="false"
            :esperado="[
              'The original name was Colombian Land. It was an homage to a bar on the base',
            ]"
            tamano="53"
          />
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            <b>Q3. </b>What is the M.F.O.? What is the organisation's purpose?
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <inputChecked
            :resuelto="false"
            :esperado="[
              'Multinational Force & Observers. It was a peacekeeping organization',
            ]"
            tamano="47"
          />
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC"><b>Q4. </b>Where was the M.F.O based?</h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <inputChecked
            :resuelto="false"
            :esperado="['It was based in Rome']"
            tamano="21"
          />
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            <b>Q5. </b>How many bars were there at the base? What did the
            soldiers do at the bars?
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <inputChecked
            :resuelto="false"
            :esperado="[
              'There were 12 bars on the base. The soldiers would enjoy each other',
            ]"
            tamano="47.3"
          />
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            <b>Q6. </b>How long after seeing the sign for English classes was
            the director hired? When did he start work?
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <inputChecked
            :resuelto="false"
            :esperado="[
              'He was hired on the same day as seeing the sign and started work the very next morning',
            ]"
            tamano="59"
          />
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            <b>Q7. </b>Who helped with the director's dream of forming the
            school?
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <inputChecked
            :resuelto="false"
            :esperado="['Seth Goodrow helped with the director’s dream']"
            tamano="34.4"
          />
        </b-col>
      </b-row>
      <br />
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
      tabla5P7: {
        fields: [
          { key: "a", thClass: "noHead" },
          { key: "b", thClass: "noHead" },
        ],
        items: [
          { a: "Beginning", b: "Inicio" },
          { a: "Join", b: "Unir" },
          { a: "Chosen", b: "Participio de choose (elegir)" },
          { a: "Among", b: "Entre" },
          { a: "Several", b: "Varios" },
          { a: "In early", b: "A principios" },
          { a: "Headquartered", b: "Localizado en" },
          { a: "Agreement", b: "Acuerdo" },
          { a: "Peacekeeping", b: "Preservacion de la paz" },
          { a: "Settle down", b: "Establecerse, radicarse" },
          { a: "On the way out", b: "De salida" },
          { a: "Sign", b: "Firmar, señal, aviso" },
          { a: "Younger", b: "Más joven" },
          { a: "Hire", b: "Contratar" },
          { a: "Go by", b: "Pasar" },
          { a: "Hand over", b: "Entregar" },
          { a: "Come into fruition", b: "Dar frutos" },
          { a: "Homage", b: "Homenaje" },
          { a: "Rename", b: "Renombrar" },
          { a: "Whereas", b: "Mientras que" },
          { a: "Grow", b: "Crecer" },
          { a: "Surely", b: "Con toda certeza" },
        ],
      },
    };
  },
};
</script>
