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
      <b-col sm="auto">
        <tablaTC :cuestionario="tabla1P52" />
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
          { key: "html1", label: "2", thClass: "noHead" },
          { key: "html1", label: "3", thClass: "noHead" }
        ],
        items: [
          {
            html1: "I <span class='colorLetraRojo'>have got</span> a car",
            html1: "I <span class='colorLetraRojo'>haven't got</span> a car",
            html1: "<span class='colorLetraRojo'>Have</span> you <span class='colorLetraRojo'>got</span> a car? "
          },
        ],
      },
    };
  },
};
</script>

<style>
</style>