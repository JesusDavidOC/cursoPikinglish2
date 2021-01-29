<template>
  <b-container fluid>
    <b-row> 
        <inputCE :object="inputCheckedprueba"/>
    </b-row>
  </b-container>
</template>

<script>
import inputCE from "./inputCEnriquecido";
export default {
  components: {
    inputCE,
  },
  data() {
    return {
        inputCheckedprueba:{
            lista1:["su mama"],
            name:"inputChekedpruebas1",
            textoA:"pruebita",
            textoD:"pruebita",
            tamano1:20,
            lista2:["la suya"],
            textoD2:":3",
            tamano2:20,
        }
    };
  },
};
</script>

<style>
</style>