<template>
  <div>
    <b-container fluid>
      <b-row>
        <b-col></b-col>
        <b-col sm="auto">
          <h3 class="titulo">THE USE OF THERE.</h3>
        </b-col>
        <b-col></b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            Esta palabra es un adverbio de lugar que traduce “allá o ahí” pero
            se usa de muchas maneras más al agregarle un verbo con poder o un
            auxiliar y a continuación veremos las conjugaciones.
          </h3>
        </b-col>
      </b-row>
      <br /><br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="10">
          <tablaTC :cuestionario="tabla3P7" />
        </b-col>
      </b-row>
      <br /><br />

      <b-row>
        <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            Complete with the right “there + s.p.v or Aux.”
          </h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3>
            <b>HAY</b>
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            Should we go into that restaurant? It looks nice, but
          </h3>
        </b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['there is']"
            tamano="12.3"
          />
        </b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            only one person in there.
          </h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3>
            <b>HAY</b>
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['There are', 'there are']"
            tamano="12.3"
          />
        </b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            enough cookies here for the whole class to share.
          </h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3>
            <b>HUBO</b>
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            I wanted to go and see more sights in Rome, but
          </h3>
        </b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['there was']"
            tamano="12.3"
          />
        </b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            no time for me to do that, and
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            buy souvenirs and get to the airport in time.
          </h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3>
            <b>HUBO</b>
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['there were', 'There were']"
            tamano="12.3"
          />
        </b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            so many people in the nightclub last night. I felt like a canned
            sardine at times.
          </h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3>
            <b>HABRÁ</b>
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            By the time the war ends
          </h3>
        </b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['there will be']"
            tamano="12.3"
          />
        </b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            bodies everywhere.
          </h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3>
            <b>HABRIÁ</b>
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['There would be']"
            tamano="13"
          />
        </b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            no need for a cake and alcohol if we were to have a party.
          </h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3>
            <b>VA A HABER </b>
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['There is going to be']"
            tamano="15.5"
          />
        </b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            a lot of trouble if your mum finds out what you’ve done.
          </h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3>
            <b>IBA A HABER </b>
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['There was going to be']"
            tamano="17"
          />
        </b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            a clown at my birthday party, but he canceled at the last minute.
          </h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3>
            <b>TIENE QUE HABER</b>
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['There has to be']"
            tamano="13.5"
          />
        </b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            some coffee in this kitchen.
          </h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3>
            <b>PUEDE HABER</b>
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            Of course, go for a walk in the jungle, but just remember that
          </h3>
        </b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['there may be']"
            tamano="12.3"
          />
        </b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            a lot of dangers in there.
          </h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3>
            <b>PODRÍA HABER</b>
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            There’s a food festival in town today. Shall we go? Because
          </h3>
        </b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['there might be']"
            tamano="13"
          />
        </b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            Mexican food available.
          </h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3>
            <b>DEBERÍA HABER</b>
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            I’m going on a skiing holiday next week. I know it’s been warm here
            recently, but
          </h3>
        </b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['there should be']"
            tamano="13.7"
          />
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            lots of snow up in the mountains of France.
          </h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3>
            <b>NECESITA HABER-ES NECESARIO QUE HAYA</b>
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            The curriculum is really good, but
          </h3>
        </b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['there needs to be']"
            tamano="14.6"
          />
        </b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            a high standard of teachers available for the students.
          </h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3>
            <b>DEBE HABER</b>
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            I saw so many poor people on the streets,
          </h3>
        </b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['there must be']"
            tamano="13"
          />
        </b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            something we can do to help them.
          </h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3>
            <b>PARECE HABER/ PARECE QUE HAY</b>
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            I paid for my shopping this morning but
          </h3>
        </b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['there seems to be']"
            tamano="15"
          />
        </b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            something wrong because it cost a lot more
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            than I thought it would.
          </h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3>
            <b>HA HABIDO</b>
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            Terrible news this morning,
          </h3>
        </b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['there has been']"
            tamano="13.5"
          />
        </b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            an Earthquake in New Zealand and a lot of people hav died.
          </h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3>
            <b>HABRÍA HABIDO</b>
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['There would have been']"
            tamano="18"
          />
        </b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            a lot more injured people if Spider-Man hadn’t stopped the Green
            Goblin.
          </h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3>
            <b>PODRÍA HABER HABIDO</b>
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            The picture was really dull. There
          </h3>
        </b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['might have been']"
            tamano="14.3"
          />
        </b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            a lot more colors and it would have looked so much
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            more vibrant.
          </h3>
        </b-col>
      </b-row>
      <br />

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3>
            <b>DEBERÍA/DEBIÓ O DEBE HABER HABIDO</b>
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            I went to class today and
          </h3>
        </b-col>
        <b-col sm="left">
          <inputChecked
            :resuelto="false"
            :esperado="['there should have been']"
            tamano="18.3"
          />
        </b-col>
        <b-col sm="auto">
          <h3 class="parrafoIC">
            ten students in the classroom, but only three
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            people came because it was raining.
          </h3>
        </b-col>
      </b-row>
      <br /><br />

      <b-row>
        <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            Choose the right option
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="10">
          <opcionMultiple
            :options="$data.cuestionarioP17"
            :rEsperadas="$data.respuestasCuestionarioP17"
            :respuestas="$data.mensajeRespuestasP17 = $event"
          />
        </b-col>
        <b-col class="col-sm-1"></b-col>
        <b-modal ref="my-modal1" hide-footer title="RESULTADO">{{
          mensajeRespuestasP17
        }}</b-modal>
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
      cuestionarioP17: [
        {
          respuesta: "",
          pregunta: "1. Creo que debe haber un error en la cuenta.	I think ________ be a mistake on the bill.",
          options: [
            {
              text: "A) There is",
              value: "A",
              disabled: false,
            },
            {
              text: "B) there has been",
              value: "B",
              disabled: false,
            },
            {
              text: "C) there must be",
              value: "C",
              disabled: false,
            },
          ],
        },
        {
          respuesta: "",
          pregunta: "2. Me dijeron que habría un concierto.I was told______be a concert",
          options: [
            {
              text: "A) There will be",
              value: "A",
              disabled: false,
            },
            {
              text: "B) there could be",
              value: "B",
              disabled: false,
            },
            {
              text: "C) there would be",
              value: "C",
              disabled: false,
            },
          ],
        },
        {
          respuesta: "",
          pregunta: "3. No hay nada que hacer. _____ nothing to do. ",
          options: [
            {
              text: "A) There are",
              value: "A",
              disabled: false,
            },
            {
              text: "B)  there is ",
              value: "B",
              disabled: false,
            },
            {
              text: "C) there",
              value: "C",
              disabled: false,
            },
          ],
        },
        {
          respuesta: "",
          pregunta: "4. Debe haber algo que podamos hacer para evitar vender el carro. ____________ something we can do to avoid selling the car.",
          options: [
            {
              text: "A) There is going to be",
              value: "A",
              disabled: false,
            },
            {
              text: "B) there must be",
              value: "B",
              disabled: false,
            },
            {
              text: "C) there must have been",
              value: "C",
              disabled: false,
            },
          ],
        },
        {
          respuesta: "",
          pregunta: "5. La fiesta fue un desastre, debería haber habido una persona responsable de la logística. The party was a mess, __________ a person in charge of logistics.",
          options: [
            {
              text: "A) There should be",
              value: "A",
              disabled: false,
            },
            {
              text: "B) there should have be",
              value: "B",
              disabled: false,
            },
            {
              text: "C) there should have been",
              value: "C",
              disabled: false,
            },
          ],
        },
        {
          respuesta: "",
          pregunta: "6. Podría haber una gran tormenta en la noche. ___________ huge storm tonight",
          options: [
            {
              text: "A) There is going to be",
              value: "A",
              disabled: false,
            },
            {
              text:
                "B) there can be",
              value: "B",
              disabled: false,
            },
            {
              text: "C) there might be",
              value: "C",
              disabled: false,
            },
          ],
        },
      ],
      respuestasCuestionarioP17: ["C", "C", "B", "B", "C", "C"],
      mensajeRespuestasP17: "",

      tabla3P7: {
        fields: [
          { key: "html1", thClass: "noHead" },
          { key: "b", thClass: "noHead" },
          { key: "c", thClass: "noHead" },
        ],
        items: [
          {
            html1: "<b>There is</b>",
            b: "Hay (Singular) ",
            c: "There is a cat in the window",
          },
          {
            html1: "<b>There are</b>",
            b: "Hay (Plural)",
            c: "There are children at the park",
          },
          {
            html1: "<b>There was</b>",
            b: "Hubo",
            c: "There was an accident on the road",
          },
          {
            html1: "<b>There were</b>",
            b: "Hubo (Plural)",
            c: "There were no flowers left",
          },
          {
            html1: "<b>There will be</b>",
            b: "Habrá",
            c: "There will be fireworks on Friday",
          },
          {
            html1: "<b>There is going to be</b>",
            b: "Va A Haber",
            c: "There is going to be many more opportunities",
          },
          {
            html1: "<b>There was going to be</b>",
            b: "Iba A Haber ",
            c: "There was going to be a concert",
          },
          {
            html1: "<b>There would be</b>",
            b: "Habría",
            c: "There would be a consequence",
          },
          {
            html1: "<b>There has to be</b>",
            b: "Tiene Que Haber",
            c: "There has to be another way to get out!",
          },
          {
            html1: "<b>There needs to be</b>",
            b: "Debe Haber, Tiene Que Haber, Es Necesario, Se Necesita",
            c: "There needs to be security at the door",
          },
          {
            html1: "<b>There seems to be</b>",
            b: "Parece Haber",
            c: "There seems to be a problem with the computer",
          },
          {
            html1: "<b>There might be</b>",
            b: "Podría Haber",
            c: "Watch out! There might be a snake over there",
          },
          {
            html1: "<b>There may be</b>",
            b: "Pude Que Haya, Puede Haber",
            c: "There may be a monster in the wardrobe",
          },
          {
            html1: "<b>There can be</b>",
            b: "Puede Haber",
            c: "There can be only 3 people in the lift/elevator",
          },
          {
            html1: "<b>There could be</b>",
            b: "Pudo Haber",
            c: "There could be people I know at the party",
          },
          {
            html1: "<b>There should be</b>",
            b: "Debería Haber",
            c: "There should be a fire alarm in the flat",
          },
          {
            html1: "<b>There must be</b>",
            b: "Debe Haber",
            c: "There must be a cake for the wedding",
          },
          {
            html1: "<b>There has been</b>",
            b: "Ha Habido ",
            c: "There has been a theft!",
          },
          {
            html1: "<b>There had been</b>",
            b: "Había habido",
            c: "There had been a murder at the graveyard",
          },
          {
            html1: "<b>There would have been</b>",
            b: "Habría Habido",
            c: "There would have been a BBQ if it weren't for the rain",
          },
          {
            html1: "<b>There should have been</b>",
            b: "Debería Haber Habido",
            c: "There should have been an adult with the child",
          },
        ],
      },
    };
  },
};
</script>
