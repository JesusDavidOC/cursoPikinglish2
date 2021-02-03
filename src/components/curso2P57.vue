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
          @respuestas="$data.mensajeRespuestasP101 = $event"
        />
        <b-button variant="primary" @click="showModal('my-modalP62')"
          >VERIFICAR PREGUNTAS</b-button>
        <b-modal ref="my-modalP62" hide-footer title="RESULTADO">{{
          mensajeRespuestasP62
        }}</b-modal>
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
import inputCE from "./inputCEnriquecido";
import tablaTC from "./tablaTraduccionCodigos";
import opcionMultiple from "./opcionMultiple";
export default {
  components: {
    inputCE,
    tablaTC,
    opcionMultiple,
  },
  data() {
    return {
      mensajeRespuestasP62: "Complete las preguntas",
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
          pregunta: "9. It ___ (taste) delicious, but you didn’t add sugar.",
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
    };
  },
};
</script>

<style>
</style>