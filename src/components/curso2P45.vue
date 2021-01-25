<template>
  <b-container fluid>
    <b-row>
      <b-col sm="auto">
        <h3 class="subTitulo">PEDIR CONSENTIMIENTO</h3>
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="auto">
        <tablaTC :cuestionario="tabla1P45" />
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
      tabla1P45: {
        fields: [
          { key: "null", label: "verbo", thClass: "noHead" },
          { key: "html1", label: "pruebita :3", thClass: "noHead" },
        ],
        items: [
            {null:"¿Bailamos?",html1:"<span>Shall</span> we dance?"}
        ],
      },
    };
  },
};
</script>

<style>
</style>