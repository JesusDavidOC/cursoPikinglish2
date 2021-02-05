<template>
  <b-container>
    <b-row>
      <b-col></b-col>
      <b-col sm="auto">
        <h3 class="titulo">Otras Fusiones de verbos con super poder</h3>
      </b-col>
      <b-col></b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="10">
        <p class="parrafo">
          Estos temas de gramática avanzada pueden entenderse sencillamente con
          lógica al unir las siguientes partes.
        </p>
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="10">
        <tablaTC :cuestionario="tabla1P61" />
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="10">
        <tablaTC :cuestionario="tabla2P61" />
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="auto">
        <h3 class="subTitulo">Examples</h3>
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="10">
        <p class="parrafo">
          ° He <strong>could have</strong> fallen down the stairs (Él pudo
          haberse caído de las escaleras)
        </p>
        <p class="parrafo">
          ° She <strong>would have</strong> cooked something (Ella habría
          cocinado algo)
        </p>
        <p class="parrafo">
          ° You <strong>should</strong> have come, you missed it (Tú debiste
          haber venido, te lo perdiste)
        </p>
        <p class="parrafo">
          ° What<strong> would</strong> you <strong>have</strong> done? (¿Qué
          habrías hecho?)
        </p>
        <p class="parrafo">
          ° What<strong> should I have</strong> done then? (¿Qué debería haber
          hecho entonces?)
        </p>
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="auto">
        <h3 class="subTitulo">
          Listen and complete the sentence with the verb in the right spelling
          form.
        </h3>
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="10">
        <opcionMultiple
          :options="$data.cuestionarioP62"
          :rEsperadas="$data.respuestasCuestionarioP62"
          @respuestas="$data.mensajeRespuestasP62 = $event"
        />
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="auto">
        <h3 class="subTitulo">Pick the right spanish translation</h3>
      </b-col>
    </b-row>
    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="10">
        <opcionMultiple
          :options="$data.cuestionarioP63"
          :rEsperadas="$data.respuestasCuestionarioP63"
          @respuestas="$data.mensajeRespuestasP63 = $event"
        />
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="auto">
        <h3 class="subTitulo">Put in order</h3>
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="10">
        <b-row
          v-for="(item, index) in listadoCompletarP63"
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
    <b-row>
      <b-col sm="auto">
        <h3 class="subTitulo">
          Fill in the gaps to complete the right English translation.
        </h3>
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="11">
        <b-row
          v-for="(item, index) in listadoCompletar2P63"
          :key="index + item.textoA"
          class="margin-bottom"
        >
          <b-col><inputCE :object="item" /></b-col>
        </b-row>
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
import inputChecked from "./inputChecked";
import inputCE from "./inputCEnriquecido";
import tablaTC from "./tablaTraduccionCodigos";
import opcionMultiple from "./opcionMultiple";
export default {
  components: {
    inputChecked,
    inputCE,
    tablaTC,
    opcionMultiple,
  },
  data() {
    return {
      listadoCompletar2P63: [
        {
          lista1: ["could"],
          name: "inputCheked2",
          textoA: "1. Ellos pudieron haber ganado / they ",
          textoD: "",
          tamano1: 34,
          lista2: ["have"],
          textoD2: "won",
          tamano2: 10.4,
        },
        {
          lista1: ["should"],
          name: "inputCheked2",
          textoA: "2. Nadie debió haberse ido aún / Nobody",
          textoD: "",
          tamano1: 36.8,
          lista2: ["have"],
          textoD2: "gone yet",
          tamano2: 13.4,
        },
        {
          lista1: ["could"],
          name: "inputCheked2",
          textoA: "3. Él pudo haber sido el ganador / He",
          textoD: "",
          tamano1: 33.8,
          lista2: ["have"],
          textoD2: "been the winner",
          tamano2: 18,
        },
        {
          lista1: ["would"],
          name: "inputCheked2",
          textoA: "4. Si yo fuese tú, habría ido a la fiesta. / If I were you, I",
          textoD: "",
          tamano1: 47.4,
          lista2: ["have"],
          textoD2: "gone to the party.",
          tamano2: 18.9,
        },
        {
          lista1: ["could"],
          name: "inputCheked2",
          textoA: "5. Si hubiese tenido dinero, podría haber ido a la Universidad. / If I had had some money, I",
          textoD: "",
          tamano1: 69,
          lista2: ["have"],
          textoD2: "gone to university.",
          tamano2: 19.8,
        },
        {
          lista1: ["should"],
          name: "inputCheked2",
          textoA: "6. No debiste haberle dicho a ella nada. / You",
          textoD: "not",
          tamano1: 41.8,
          lista2: ["have"],
          textoD2: "told her anything.",
          tamano2: 18.9,
        },
        {
          lista1: ["would"],
          name: "inputCheked2",
          textoA: "7. ¿Qué habrías hecho? / What",
          textoD: "you",
          tamano1: 32.4,
          lista2: ["have"],
          textoD2: "done?",
          tamano2: 12,
        },
        {
          lista1: ["should"],
          name: "inputCheked2",
          textoA: "8. No debiste haber ido sin avisar. / You",
          textoD: "not",
          tamano1: 38,
          lista2: ["have"],
          textoD2: "left without saying good-bye",
          tamano2: 26,
        },
      ],
      respuestasCuestionarioP63: ["C", "B", "C"],
      cuestionarioP63: [
        {
          respuesta: "",
          pregunta: "1. I would have liked to do that.",
          options: [
            {
              text: "A)  Me gustaría eso",
              value: "A",
              disabled: false,
            },
            {
              text: "B) Me ha gustado eso",
              value: "B",
              disabled: false,
            },
            {
              text: "C) Me habría gustado hacer eso",
              value: "C",
              disabled: false,
            },
          ],
        },
        {
          respuesta: "",
          pregunta: "2. They shouldn’t have let him in ",
          options: [
            {
              text: "A)  Ellos deberían dejarlo entrar",
              value: "A",
              disabled: false,
            },
            {
              text: "B) No deberían haberlo dejado entrar",
              value: "B",
              disabled: false,
            },
            {
              text: "C) Ellos no deberían haberle permitido irse ",
              value: "C",
              disabled: false,
            },
          ],
        },
        {
          respuesta: "",
          pregunta: "3. He could have been a super star",
          options: [
            {
              text: "A)  Él pudo ser una super Estrella",
              value: "A",
              disabled: false,
            },
            {
              text: "B) él ha sido una super estrella ",
              value: "B",
              disabled: false,
            },
            {
              text: "C) él pudo haber sido una super estrella",
              value: "C",
              disabled: false,
            },
          ],
        },
      ],
      respuestasCuestionarioP62: [
        "B",
        "A",
        "B",
        "B",
        "A",
        "B",
        "B",
        "B",
        "A",
        "A",
      ],
      cuestionarioP62: [
        {
          respuesta: "",
          pregunta: "1. I ___ (do) that.",
          audio: "",
          options: [
            {
              text: "A) would have done",
              value: "A",
              disabled: false,
            },
            {
              text: "B) could have done",
              value: "B",
              disabled: false,
            },
            {
              text: "C) whould have do",
              value: "C",
              disabled: false,
            },
          ],
        },
        {
          respuesta: "",
          pregunta: "2. You ___ (eat) healthy food.",
          audio: "",
          options: [
            {
              text: "A) should have eaten",
              value: "A",
              disabled: false,
            },
            {
              text: "B) would have eat",
              value: "B",
              disabled: false,
            },
            {
              text: "C) could have eaten",
              value: "C",
              disabled: false,
            },
          ],
        },
        {
          respuesta: "",
          pregunta: "3. He ___ (win) the competition",
          audio: "",
          options: [
            {
              text: "A) should have win",
              value: "A",
              disabled: false,
            },
            {
              text: "B) could have won",
              value: "B",
              disabled: false,
            },
            {
              text: "C) would have won",
              value: "C",
              disabled: false,
            },
          ],
        },
        {
          respuesta: "",
          pregunta: "4. They ___ (arrive) by now.",
          audio: "",
          options: [
            {
              text: "A) could have arrive",
              value: "A",
              disabled: false,
            },
            {
              text: "B) hould have arrived",
              value: "B",
              disabled: false,
            },
            {
              text: "C) would have arrive",
              value: "C",
              disabled: false,
            },
          ],
        },
        {
          respuesta: "",
          pregunta: "5. We ___ (go) to the gym.",
          audio: "",
          options: [
            {
              text: "A) should have gone",
              value: "A",
              disabled: false,
            },
            {
              text: "B) could have gone",
              value: "B",
              disabled: false,
            },
            {
              text: "C) would have gone",
              value: "C",
              disabled: false,
            },
          ],
        },
        {
          respuesta: "",
          pregunta: "6. She ___ (be) a very good actress.",
          audio: "",
          options: [
            {
              text: "A) would have be",
              value: "A",
              disabled: false,
            },
            {
              text: "B) could have been",
              value: "B",
              disabled: false,
            },
            {
              text: "C) should have been",
              value: "C",
              disabled: false,
            },
          ],
        },
        {
          respuesta: "",
          pregunta: "7. I ___ (laugh) if I knew he was joking.",
          audio: "",
          options: [
            {
              text: "A) could have laughed ",
              value: "A",
              disabled: false,
            },
            {
              text: "B) would have laughed ",
              value: "B",
              disabled: false,
            },
            {
              text: "C) should have laughed ",
              value: "C",
              disabled: false,
            },
          ],
        },
        {
          respuesta: "",
          pregunta: "8. it  ___ (finish) by now if it started at 8pm",
          audio: "",
          options: [
            {
              text: "A) should have finish",
              value: "A",
              disabled: false,
            },
            {
              text: "B) would have finished ",
              value: "B",
              disabled: false,
            },
            {
              text: "C) could have finished ",
              value: "C",
              disabled: false,
            },
          ],
        },
        {
          respuesta: "",
          pregunta: "9. We ___ (die) if we drove in that weather.",
          audio: "",
          options: [
            {
              text: "A) would have died",
              value: "A",
              disabled: false,
            },
            {
              text: "B) hould have died ",
              value: "B",
              disabled: false,
            },
            {
              text: "C) could have died ",
              value: "C",
              disabled: false,
            },
          ],
        },
        {
          respuesta: "",
          pregunta: "10. It ___ (taste) delicious, but you didn’t add sugar.",
          audio: "",
          options: [
            {
              text: "A) could have tasted",
              value: "A",
              disabled: false,
            },
            {
              text: "B) should have taste",
              value: "B",
              disabled: false,
            },
            {
              text: "C) would have tasted",
              value: "C",
              disabled: false,
            },
          ],
        },
      ],
      tabla1P61: {
        fields: [
          { key: "col1", label: " ", thClass: "noHead" },
          { key: "html1", label: " ", thClass: "noHead" },
          { key: "col4", label: " ", thClass: "noHead" },
        ],
        items: [
          {
            col1: "Would",
            html1: "<span class='colorLetraRojo'>Have + participle</span>",
            col4: "Habría",
          },
          {
            col1: "Could",
            html1: "<span class='colorLetraRojo'>Have + participle</span>",
            col4: "Pude, Podría haber",
          },
          {
            col1: "Should",
            html1: "<span class='colorLetraRojo'>Have + participle</span>",
            col4: "Debería haber",
          },
        ],
      },
      tabla2P61: {
        fields: [
          { key: "sup", label: "sup", thClass: "" },
          { key: "aux", label: "aux", thClass: "" },
          { key: "spv", label: "s.p.v", thClass: "" },
          { key: "participle", label: "participle", thClass: "" },
          { key: "Translation", label: "Translation", thClass: "" },
        ],
        items: [
          {
            sup: "I",
            aux: "would",
            spv: "have",
            participle: "had",
            Translation: "Yo habría tenido ",
          },
          {
            sup: "I",
            aux: "could",
            spv: "have",
            participle: "done",
            Translation: "Yo pude haber hecho",
          },
          {
            sup: "I",
            aux: "should",
            spv: "have",
            participle: "eaten",
            Translation: "Yo debería haber comido",
          },
        ],
      },
      listadoCompletarP63: [
        {
          listado: ["What do you think I should have done"],
          textoA: "1. YOU/DO/WHAT/SHOULD/HAVE/THINK/I/DONE? ",
          textoD: "",
          tamano: "62",
        },
        {
          listado: ["I could have been the king"],
          textoA: "2. I/HAVE/BEEN/COULD/THE KING ",
          textoD: "",
          tamano: "45",
        },
        {
          listado: ["What would you have done?"],
          textoA: "3. WOULD/YOU/WHAT/DONE? /HAVE",
          textoD: "",
          tamano: "50.8",
        },
        
      ],
    };
  },
};
</script>

<style>
</style>