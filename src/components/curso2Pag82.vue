<template>
  <div>
    <b-container fluid>
      <b-row>
        <b-col></b-col>
        <b-col sm="auto">
          <h3 class="titulo">YES- NO QUESTIONS</h3>
        </b-col>
        <b-col></b-col>
      </b-row>

      <b-row class="diamondContainer">
        <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
        <b-col>
          <h3 class="fuenteDiamond">
            Las preguntas que empiezan con un auxiliar o verbo con súper poder
            se llaman YES-NO QUESTIONS porque su respuesta es siempre
            <b>SI O NO.</b>
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="11">
          <h3 class="subTitulo">FORMAS DE RESPONDER PREGUNTAS CON SI O NO.</h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            <b>1. </b>Respuesta completa. Es decir que se responde incluyendo el
            contenido de la pregunta.
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            <br />
            <b>- </b>Are you working today? Yes, I am working today <br /><br />
            <b>- </b>Can you please help me do my homework? No, I can´t help you
            do your homework <br /><br />
            <b>- </b>Is it going to rain? Yes, it is going to rain
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            <br />
            <b>2. </b>Respuesta corta. Es decir que solo se responde con el
            sujeto personal (I, YOU, SHE, HE, IT, WE, THEY) más el auxiliar o
            verbo con súper poder.
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            <br />
            <b>- </b> <span class="colorLetraRojo">Have</span> you been working
            hard? Yes, I <span class="colorLetraRojo">have</span><br /><br />
            <b>- </b> <span class="colorLetraRojo">Were</span>you drinking with
            her last night? No, I <span class="colorLetraRojo"> wasn’t</span
            ><br /><br />
            <b>- </b> <span class="colorLetraRojo">Would</span> you like to come
            with me? Yes, I <span class="colorLetraRojo">would</span
            ><br /><br />
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="11">
          <h3 class="subTitulo">LET'S PRACTICE</h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            <b>1. </b> <span class="colorLetraRojo">Do </span> You understand
            what I am saying? Yes,
          </h3>
        </b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['I do', 'i do']"
            tamano="10"
          />
        </b-col>
        <b-col sm="3">
          <h3 class="parrafoIC">(short answer)</h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            <b>2. </b> <span class="colorLetraRojo">Does </span> she know the
            answer? No,
          </h3>
        </b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['she doesn’t know the answer']"
            tamano="24"
          />
        </b-col>
        <b-col sm="3">
          <h3 class="parrafoIC">(full answer)</h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            <b>3. </b> <span class="colorLetraRojo">Did </span> you go out with
            her? Yes,
          </h3>
        </b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['I did', 'i did']"
            tamano="10"
          />
        </b-col>
        <b-col sm="3">
          <h3 class="parrafoIC">(short answer)</h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            <b>4. </b> <span class="colorLetraRojo">Would </span> you do that
            for me? Yes,
          </h3>
        </b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['I would do that for you']"
            tamano="20"
          />
        </b-col>
        <b-col sm="3">
          <h3 class="parrafoIC">(full answer)</h3>
        </b-col>
      </b-row>

      <br />
      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            <b>5. </b> <span class="colorLetraRojo">Will </span>you spend the
            rest of year here in the countryside? No,
          </h3>
        </b-col>
        <b-col sm="left">
          <inputChecked :resuelto="false" :esperado="['I won’t']" tamano="12" />
        </b-col>
        <b-col sm="3">
          <h3 class="parrafoIC">(short answer)</h3>
        </b-col>
      </b-row>

      <br />
      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            <b>6. </b> <span class="colorLetraRojo">Is </span>it going to rain?
            Yes,
          </h3>
        </b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['it’s going to rain']"
            tamano="16"
          />
        </b-col>
        <b-col sm="3">
          <h3 class="parrafoIC">(full answer)</h3>
        </b-col>
      </b-row>

      <br />
      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            <b>7. </b> <span class="colorLetraRojo">Are </span>you interested in
            learning how to cook? Yes,
          </h3>
        </b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['I am', 'i am']"
            tamano="10"
          />
        </b-col>
        <b-col sm="3">
          <h3 class="parrafoIC">(short answer)</h3>
        </b-col>
      </b-row>

      <br />
      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            <b>8 . </b> <span class="colorLetraRojo">Could</span> they drive us
            home from work? No,
          </h3>
        </b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['they couldn’t']"
            tamano="15"
          />
        </b-col>
        <b-col sm="3">
          <h3 class="parrafoIC">(short answer)</h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="11">
          <h3 class="subTitulo">ANSWER THE FOLLOWING QUESTIONS</h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="10">
          <tablaTC :cuestionario="tabla3P7" />
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
      tabla3P7: {
        fields: [
          { key: "html1", label: "Question", thClasss: "noHead" },
          { key: "complejo1", label: "Positive form" },
          { key: "complejo2", label: "Negative form" },
        ],
        items: [
          {
            html1: "<span class='colorLetraRojo'>Are </span> you married?",
            complejo1: { lista: ["Yes, I am"], tamano: 13.5, resuelto: false },
            complejo2: { lista: ["No, I am not"], tamano: 15, resuelto: false },
          },
          {
            html1: "<span class='colorLetraRojo'>Have </span> you ever ridden a camel?",
            complejo1: { lista: ["Yes, I have"], tamano: 14.3, resuelto: false },
            complejo2: { lista: ["No, I haven´t"], tamano: 15, resuelto: false},
          },
          {
            html1: "<span class='colorLetraRojo'>Did</span> you look over the book?",
            complejo1: { lista: ["Yes, I did"], tamano: 13.3, resuelto: false },
            complejo2: { lista: ["No, I didn’t"], tamano: 14.3, resuelto: false },
          },
          {
            html1: "<span class='colorLetraRojo'>Is</span> that really good?",
            complejo1: { lista: ["Yes, it is"], tamano: 13, resuelto: false },
            complejo2: { lista: ["No, it isn’t"], tamano: 13.5, resuelto: false },
          },
          {
            html1: "<span class='colorLetraRojo'>Can</span> you help me with the bags?",
            complejo1: { lista: ["Yes, I can"], tamano: 13.5, resuelto: false },
            complejo2: { lista: ["No, I can’t"], tamano: 14, resuelto: false },
          },
          {
            html1: "<span class='colorLetraRojo'>Does</span> she know it?",
            complejo1: { lista: ["Yes, she does"],tamano: 16, resuelto: false},
            complejo2: { lista: ["No, she doesn’t"],tamano: 17.3,resuelto: false},
          },
          {
            html1: "<span class='colorLetraRojo'>Do</span> You understand what I am saying?",
            complejo1: { lista: ["Yes, I do"], tamano: 13, resuelto: false },
            complejo2: { lista: ["No, I don’t"], tamano: 14, resuelto: false },
          },
          {
            html1: "<span class='colorLetraRojo'>Does</span> she know the answer?",
            complejo1: {lista: ["Yes, she does"], tamano: 16, resuelto: false},
            complejo2: {lista: ["No, she doesn’t"], tamano: 17, resuelto: false},
          },
          {
            html1: "<span class='colorLetraRojo'>Could</span>	you tell me what that is?",
            complejo1: { lista: ["Yes, I can"], tamano: 13.5, resuelto: false },
            complejo2: { lista: ["No, I can’t"], tamano: 14, resuelto: false },
          },
          {
            html1: "<span class='colorLetraRojo'>Had</span> you had that incident before?",
            complejo1: { lista: ["Yes, I had "], tamano: 14, resuelto: false },
            complejo2: { lista: ["No, I hadn’t"], tamano: 14.5, resuelto: false },
          },
          {
            html1: "<span class='colorLetraRojo'>Were</span>	they talking about animals?",
            complejo1: { lista: ["Yes, they were"], tamano: 16.5, resuelto: false},
            complejo2: {  lista: ["No, they weren’t"], tamano: 17.5, resuelto: false},
          },
          {
            html1: "<span class='colorLetraRojo'>May</span> I borrow your car?",
            complejo1: { lista: ["Yes, you may"], tamano: 16, resuelto: false },
            complejo2: { lista: ["No, you may not"], tamano: 17.5, resuelto: false},
          },
          {
            html1: "<span class='colorLetraRojo'>Am</span> I right?",
            complejo1: { lista: ["Yes, you are"], tamano: 15, resuelto: false },
            complejo2: {
              lista: ["No, you are not"],
              tamano: 17,
              resuelto: false,
            },
          },
          {
            html1: "<span class='colorLetraRojo'>Would</span> you like me to come with you?",
            complejo1: { lista: ["Yes, I would"], tamano: 15.5, resuelto: false },
            complejo2: {
              lista: ["No, I wouldn’t"],
              tamano: 16,
              resuelto: false,
            },
          },
          {
            html1: "<span class='colorLetraRojo'>Can</span> I help you?",
            complejo1: { lista: ["Yes, you can"], tamano: 15.5, resuelto: false },
            complejo2: {
              lista: ["No, you can’t"],
              tamano: 16,
              resuelto: false,
            },
          },
          {
            html1: "<span class='colorLetraRojo'>Was</span> he singing loudly?",
            complejo1: { lista: ["Yes, he was"], tamano: 15, resuelto: false },
            complejo2: {
              lista: ["No, he wasn’t"],
              tamano: 16,
              resuelto: false,
            },
          },
          {
            html1: "<span class='colorLetraRojo'>Did</span> you overtake that car?",
            complejo1: { lista: ["Yes, I did"], tamano: 13.5, resuelto: false },
            complejo2: { lista: ["No, I didn’t"], tamano: 14.5, resuelto: false },
          },
          {
            html1: "<span class='colorLetraRojo'>Have</span> you ever had a nightmare?",
            complejo1: { lista: ["Yes, I have"], tamano: 14.5, resuelto: false },
            complejo2: {
              lista: ["No, I haven’t"],
              tamano: 15.5,
              resuelto: false,
            },
          },
          {
            html1: "<span class='colorLetraRojo'>Do</span> you understand what is going on?",
            complejo1: { lista: ["Yes, I do"], tamano: 13.4, resuelto: false },
            complejo2: { lista: ["No, I don’t"], tamano: 14.5, resuelto: false },
          },
          {
            html1: "<span class='colorLetraRojo'>Is</span> it good?",
            complejo1: { lista: ["Yes, it is"], tamano: 14, resuelto: false },
            complejo2: { lista: ["No, it isn’t"], tamano: 14.3, resuelto: false },
          },
        ],
      },
    };
  },
};
</script>
