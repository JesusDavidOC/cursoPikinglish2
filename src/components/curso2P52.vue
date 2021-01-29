<template>
  <b-container fluid>
    <b-row>
      <b-col></b-col>
      <b-col sm="auto">
        <h3 class="titulo">HAVE GOT</h3>
      </b-col>
      <b-col></b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="auto">
        <p class="parrafo">
          Este verbo con súper poder fusionado significa
          <strong>tener</strong> y es más usado en el inglés británico.
        </p>
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="8">
        <tablaTC :cuestionario="tabla1P52" />
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="8">
        <tablaTC :cuestionario="tabla2P52" />
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="9">
        <tablaTC :cuestionario="tabla3P52" />
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="auto">
        <h3 class="subTitulo">READING</h3>
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="10">
        <p class="parrafo">
          My boss gave me a job to do about 20 minutes ago and I've been talking
          to Sarah the entire time. I
          <span class="colorLetraRojo">had better</span> start working otherwise
          he <span class="colorLetraRojo">might </span>be angry with me. He told
          me I need to write a song about our company and I'<span
            class="colorLetraRojo"
            >ve got</span
          >
          to sing about how great he is. I don't know if I will use my guitar or
          my piano for the song, but I
          <span class="colorLetraRojo">ought to</span> play both of them to see
          which sounds the best. The song may sound silly if I have got to sing
          about him, but he’s my boss and I
          <span class="colorLetraRojo">ought to</span> do what he says. I
          <span class="colorLetraRojo">might</span> ask Sheila to sing the song
          with me, she has a beautiful voice, but I
          <span class="colorLetraRojo">had better</span> ask her soon because
          she has children and if she's to help me then she
          <span class="colorLetraRojo">may</span> need to hire a babysitter so
          she doesn't have to bring her children to record the song.
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
      tabla1P52: {
        fields: [
          { key: "html1", label: "1", thClass: "noHead" },
          { key: "html2", label: "2", thClass: "noHead" },
          { key: "html3", label: "3", thClass: "noHead" },
        ],
        items: [
          {
            html1: "I <span class='colorLetraRojo'>have got</span> a car",
            html2: "I <span class='colorLetraRojo'>haven't got</span> a car",
            html3:
              "<span class='colorLetraRojo'>Have</span> you <span class='colorLetraRojo'>got</span> a car? ",
          },
          {
            html1: "I <span class='colorLetraRojo'>have</span> a car",
            html2: "I <span class='colorLetraRojo'>don't</span> have a car",
            html3: "<span class='colorLetraRojo'>Do</span> you have a car? ",
          },
        ],
      },

      tabla2P52: {
        fields: [
          { key: "amarillo", label: " ", thClass: "Yelow" },
          { key: "azul", label: " ", thClass: "Blue" },
          { key: "rojo", label: " ", thClass: "Red" },
          { key: "verde", label: " ", thClass: "Green" },
        ],
        items: [
          {
            amarillo: "1. I",
            azul: "1.Have got ",
            rojo: "1.To ",
            verde: "2.Go ",
          },
          {
            amarillo: "3. She ",
            azul: "4. Has got ",
            rojo: "2. something ",
            verde: "3. to do  ",
          },
          {
            amarillo: "5. Has",
            azul: "6. You got ",
            rojo: "4. A car? ",
            verde: "5. To tell me ? ",
          },
          {
            amarillo: "7. have ",
            azul: "8. she got  ",
            rojo: "6. a child ",
            verde: "",
          },
          {
            amarillo: "",
            azul: "10. Haven´t got ",
            rojo: "7. Anything ",
            verde: "",
          },
        ],
      },
      tabla3P52: {
        fields: [
          { key: "amarillo", label: " ", thClass: "Yelow" },
          { key: "azul", label: " ", thClass: "Blue" },
          { key: "rojo", label: " ", thClass: "Red" },
          { key: "verde", label: " ", thClass: "Green" },
          { key: "complejo1", label: "ENGLISH", thClass: "" },
          { key: "html1", label: "SPANISH ", thClass: "" },
        ],
        items: [
          {
            amarillo: "1",
            azul: "1",
            rojo: "1",
            verde: "2",
            complejo1: {
              lista: ["I have got to go"],
              tamano: 18,
              resultado: false,
            },
            html1: "<strong>Tengo que ir</strong>",
          },
          {
            amarillo: "3",
            azul: "4",
            rojo: "2",
            verde: "3",
            complejo1: {
              lista: ["She has got something to do"],
              tamano: 25.4,
              resultado: false,
            },
            html1: "<strong>Ella tiene algo que hacer </strong>",
          },
          {
            amarillo: "5",
            azul: "8",
            rojo: "4",
            verde: "",
            complejo1: {
              lista: ["Has she got a child"],
              tamano: 20,
              resultado: false,
            },
            html1: "<strong>¿Tiene ella un carro?</strong>",
          },
          {
            amarillo: "7",
            azul: "6",
            rojo: "1",
            verde: "2",
            complejo1: {
              lista: ["Have you got to go?"],
              tamano: 20.3,
              resultado: false,
            },
            html1: "<strong>¿Tienes que ir?</strong>",
          },
          {
            amarillo: "7",
            azul: "6",
            rojo: "2",
            verde: "5",
            complejo1: {
              lista: ["Have you got something to tell me?"],
              tamano: 28.4,
              resultado: false,
            },
            html1: "<strong>¿Tienes algo que contarme?</strong>",
          },
          {
            amarillo: "1",
            azul: "10",
            rojo: "6",
            verde: "",
            complejo1: {
              lista: ["I haven’t got a child"],
              tamano: 20,
              resultado: false,
            },
            html1: "<strong>Yo no tengo un hijo</strong>",
          },
        ],
      },
    };
  },
};
</script>

<style>
</style>