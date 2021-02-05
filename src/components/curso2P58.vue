<template>
  <b-container>
    <b-row>
      <b-col></b-col>
      <b-col sm="auto">
        <h3 class="titulo">CONVERSIÓN DE SONIDOS DEL INGLÉS AL ESPAÑOL</h3>
      </b-col>
      <b-col></b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="10">
        <p class="parrafo">
          Aprende algunas conversiones de sonidos de letras o sílabas del inglés
          al español. Siempre hay excepciones.
        </p>
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="10">
        <tablaTC :cuestionario="tabla1P64" />
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="auto">
        <h3 class="subTitulo">Listening exercises:</h3>
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="10">
        <p class="parrafo">Example:</p>
        <b-row>
          <b-col sm="1"></b-col>
          <b-col sm="auto">
            <p class="parrafo">° (H) Hit: I couldn’t <u>hit</u> the ball</p>
            <p class="parrafo">° (PH) Photo: Take a <u>photo</u> of me</p>
            <p class="parrafo">
              ° (GH) Tough: That exercise was really <u>tough</u>
            </p>
            <p class="parrafo">° (CH) Ache: My whole body <u>aches</u></p>
            <p class="parrafo">° (KN) Knife: I need a <u>knife</u> and fork</p>
            <p class="parrafo">° (TH) Throw: <u>Throw </u>the ball to him</p>
            <p class="parrafo">
              ° (Y) You: <u>You</u> and I are perfect together
            </p>
            <p class="parrafo">
              ° (J) Jump: I love watching her <u>jump</u> up and down
            </p>
            <p class="parrafo">
              ° (GHT) Thought: I <u>thought</u> you said you were happy!
            </p>
          </b-col>
        </b-row>
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="10">
        <p class="parrafo">
          El inglés no es un idioma fonético, esto significa que cuando hay una
          letra o un grupo de letras no será necesariamente siempre pronunciada
          de la misma manera en cada palabra. Hay unos símbolos fonéticos para
          cada sonido y por eso es importante familiarizarse con los sonidos del
          inglés.
        </p>
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="10">
        <tablaTC :cuestionario="tabla2P64" />
        <p>
          <i
            >Ver video de Alfabeto fonético internacional IPA (International
            Phonetic Alphabet)
          </i>
        </p>
      </b-col>
    </b-row>
    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="10">
        <p class="parrafo">Example:</p>
        <b-row>
          <b-col sm="1"></b-col>
          <b-col sm="auto">
            <p class="parrafo">° Kangaroo (Kangaruu)</p>
            <p class="parrafo">° Hear (Hiir)</p>
            <p class="parrafo">° Could (cuud)</p>
            <p class="parrafo">° Thief (thiif)</p>
            <p class="parrafo">° Ache (Eik</p>
            <p class="parrafo">° Cook (cuk)</p>
            <p class="parrafo">° Head (hed)</p>
            <p class="parrafo">° South (Sauth)</p>
            <p class="parrafo">° Pie (Pai)</p>
            <p class="parrafo">° Sea (sii)</p>
          </b-col>
        </b-row>
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="10">
        <p class="parrafo">
          En el idioma inglés el sonido de las letras
          <strong>B, V Y TH </strong>deben pronunciarse como lo muestra la
          imagen.<br />
          <img src="imagen(subir al server)" />
        </p>
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="10">
        <p class="parrafo">LISTENING:</p>
        <b-row>
          <b-col sm="1"></b-col>
          <b-col sm="auto">
            <p class="parrafo">° <span class="colorLetraRojo">B</span>ury</p>
            <p class="parrafo">° <span class="colorLetraRojo">B</span>ig</p>
            <p class="parrafo">° <span class="colorLetraRojo">B</span>ecause</p>
            <p class="parrafo">
              ° <span class="colorLetraRojo">B</span>rilliant
            </p>
            <p class="parrafo">° Rum<span class="colorLetraRojo">b</span>le</p>
            <p class="parrafo">° May<span class="colorLetraRojo">b</span>e</p>
            <p class="parrafo">° Ta<span class="colorLetraRojo">b</span>le</p>
            <p class="parrafo">
              ° Ca<span class="colorLetraRojo">b</span>binet
            </p>
            <p class="parrafo">
              ° <span class="colorLetraRojo">B</span>u<span
                class="colorLetraRojo"
                >bb</span
              >le
            </p>
            <p class="parrafo">
              ° O<span class="colorLetraRojo">b</span>jecti<span
                class="colorLetraRojo"
                >v</span
              >es
            </p>
            <p class="parrafo">° Wi<span class="colorLetraRojo">th</span></p>
          </b-col>

          <b-col sm="3"></b-col>
          <b-col sm="auto">
            <p class="parrafo">° <span class="colorLetraRojo">V</span>ery</p>
            <p class="parrafo">° <span class="colorLetraRojo">V</span>iolent</p>
            <p class="parrafo">° <span class="colorLetraRojo">V</span>isual</p>
            <p class="parrafo">° <span class="colorLetraRojo">V</span>accine</p>
            <p class="parrafo">
              ° Ad<span class="colorLetraRojo">v</span>antage
            </p>
            <p class="parrafo">° Ha<span class="colorLetraRojo">v</span>oc</p>
            <p class="parrafo">
              ° Creati<span class="colorLetraRojo">v</span>e
            </p>
            <p class="parrafo">° Lo<span class="colorLetraRojo">v</span>ely</p>
            <p class="parrafo">
              ° Conser<span class="colorLetraRojo">v</span>ati<span
                class="colorLetraRojo"
                >v</span
              >e
            </p>
            <p class="parrafo">
              ° Un<span class="colorLetraRojo">b</span>elie<span
                class="colorLetraRojo"
                >v</span
              >able
            </p>
            <p class="parrafo">° Brea<span class="colorLetraRojo">th </span></p>
          </b-col>
        </b-row>
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="auto">
        <h3 class="subTitulo">EL SONIDO DE LA SH Y CH</h3>
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="10">
        <p class="parrafo">
          muchas palabras en inglés se escriben casi igual con la diferencia de
          la sh o ch y es importante pronunciarlas correctamente o de lo
          contrario pueden confundirse los sonidos y por lo tanto el mensaje
          sería algo diferente.<br><br> <strong>CH:</strong> practica el sonido del tren:
          chu...chu...chu..chu o la canción del cha...cha...cha<br><br> <strong>SH:</strong> práctica con
          la señal de silencio poniendo el dedo índice en tu boca y ordenando
          shhhhhhh
        </p>
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
import tablaTC from "./tablaTraduccionCodigos";
export default {
  components: {
    tablaTC,
  },
  data() {
    return {
      tabla2P64: {
        fields: [
          { key: "letra", label: "Letra o grupo de letras", thClass: "" },
          { key: "html1", label: "SONIDO", thClass: "" },
          { key: "html2", label: "SONIDO", thClass: "" },
          { key: "col4", label: "", thClass: "noHead" },
        ],
        items: [
          {
            letra: "Oo",
            html1: "D<span class='colorLetraRojo'>oo</span>r (door)",
            html2: "P<span class='colorLetraRojo'>oo</span>r (puur)",
            col4:
              "Aunque ambas tienen las mismas vocales se pronuncian diferente",
          },
          {
            letra: "Ea",
            html1: "D<span class='colorLetraRojo'>ea</span>r (diar)",
            html2: "P<span class='colorLetraRojo'>ea</span>r (peer)",
            col4: "Hay más sonidos de la unión de las vocales",
          },
          {
            letra: "Ou",
            html1: "Sound (saund)",
            html2: "Source (sors) ",
            col4: "",
          },
          {
            letra: "Ie",
            html1: "Pierce (Piirs)",
            html2: "Pie (pai) ",
            col4: "",
          },
          {
            letra: "A",
            html1: "<span class='colorLetraRojo'>A</span>pple (apol)",
            html2: "<span class='colorLetraRojo'>A</span>lien (eilien)",
            col4: "",
          },
        ],
      },
      tabla1P64: {
        fields: [
          { key: "silaba", label: "Letra o sílaba en inglés", thClass: "" },
          { key: "sonido", label: "Sonido en español", thClass: "" },
          { key: "html1", label: "Example", thClass: "" },
          { key: "col4", label: "", thClass: "noHead" },
        ],
        items: [
          {
            silaba: "H",
            sonido: "J",
            html1: "<span class='colorLetraRojo'>H</span>ello",
            col4: "",
          },
          {
            silaba: "PH",
            sonido: "F",
            html1: "<span class='colorLetraRojo'>Ph</span>enomenal",
            col4: "",
          },
          {
            silaba: "GH",
            sonido: "F",
            html1: "Cou<span class='colorLetraRojo'>gh</span>",
            col4: "Al final de la palabra",
          },
          {
            silaba: "CH",
            sonido: "K",
            html1: "S<span class='colorLetraRojo'>ch</span>ool",
            col4: "La mayoría de las veces",
          },
          {
            silaba: "KN",
            sonido: "N",
            html1: "<span class='colorLetraRojo'>Kn</span>ow",
            col4: "",
          },
          {
            silaba: "TH",
            sonido: "Z",
            html1: "<span class='colorLetraRojo'>Th</span>ink",
            col4: "",
          },
          {
            silaba: "Y",
            sonido: "I",
            html1: "<span class='colorLetraRojo'>Y</span>ellow",
            col4: "",
          },
          {
            silaba: "J",
            sonido: "Y",
            html1: "<span class='colorLetraRojo'>J</span>ar",
            col4: "",
          },
          {
            silaba: "GHT",
            sonido: "T",
            html1: "bou<span class='colorLetraRojo'>ght</span>",
            col4: "",
          },
        ],
      },
    };
  },
};
</script>

<style>
</style>