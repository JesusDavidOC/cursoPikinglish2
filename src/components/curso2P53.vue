<template>
  <b-container fluid>
    <b-row>
      <b-col></b-col>
      <b-col sm="auto">
        <h3 class="titulo">FUSIÓN DE VERBOS CON SÚPER PODE</h3>
      </b-col>
      <b-col></b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="10">
        <p class="parrafo">
          A través de la lógica podemos enseñar conceptos gramaticales un poco
          complejos con una sencilla explicación.<br />
          Al unir estos tres verbos con super poderes con la palabra “Supposed
          to” esto se convierte en una fusión gramatical dando como resultado al
          español “SUPONER TENER QUE O DEBERÍA”
        </p>
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="auto">
        <h3 class="subTitulo">AM-IS-ARE + SUPPOSED TO + VERB.</h3>
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="10">
        <tablaTC :cuestionario="tabla1P53" />
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="11">
        <p class="parrafo">Example:</p>
        <b-row>
          <b-col sm="1"></b-col>
          <b-col sm="auto">
            <p class="parrafo">
              ° I <span class="colorLetraRojo"> supposed to </span> do my
              homework today / Yo debería hacer mis tareas hoy
            </p>
            <p class="parrafo">
              ° He <span class="colorLetraRojo">is supposed to</span> be here now     /  Se supone que él tiene que estar aquí ahora 
            </p>
            <p class="parrafo">
              ° You <span class="colorLetraRojo"> are not supposed to </span> smoke in here  / Se supone que no tienes que fumar aquí dentro 
            </p>
            <p class="parrafo">
              ° What <span class="colorLetraRojo"> am </span> i <span class="colorLetraRojo"> supposed</span>   to do?   /  ¿Qué se supone que eso significa? 
            </p>
            <p class="parrafo">
              ° What <span class="colorLetraRojo">is </span>that<span class="colorLetraRojo"> supposed</span>  to mean?  /  ¿Qué se supone que eso significa? 
            </p>
            <p class="parrafo">
              ° You <span class="colorLetraRojo"> are supposed to</span> be an expert / Se supone que eres un experto
            </p>
          </b-col>
        </b-row>
      </b-col>
    </b-row>


    <b-row>
      <b-col sm="auto">
        <h3 class="subTitulo">EXERCICES: Rewrite the sentences with SUPPOSED TO</h3>
      </b-col>
    </b-row>


    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="10">
        <p class="parrafo">Example: You can’t go out dancing. Be ill! (You) / <span class="colorLetraRojo">You can’t go out dancing. You’re supposed to be ill!</span></p>
      </b-col>
    </b-row>


    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="11">
        <b-row
          v-for="(item, index) in listadoCompletarP53"
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
  </b-container>
</template>

<script>
import tablaTC from "./tablaTraduccionCodigos";
import inputChecked from "./inputChecked";
export default {
  components: {
    tablaTC,inputChecked
  },
  data() {
    return {
      tabla1P53: {
        fields: [
          { key: "col1", label: " ", thClass: "noHead" },
          { key: "html1", label: " ", thClass: "noHead" },
          { key: "col3", label: " ", thClass: "noHead" },
          { key: "col4", label: " ", thClass: "noHead" },
        ],
        items: [
          {
            col1: "AM",
            html1: "<span class='colorLetraRojo'>Supposed to</span>",
            col3: "Verb (Present)",
            col4: "Se supone que tengo que… o deberías ... ",
          },
          {
            col1: "IS",
            html1: "<span class='colorLetraRojo'>Supposed to</span>",
            col3: "Verb (Present)",
            col4: "Se supone que (él, ella) tiene que … ",
          },
          {
            col1: "ARE",
            html1: "<span class='colorLetraRojo'>Supposed to</span>",
            col3: "Verb (Present)",
            col4: "Se supone que tenemos, tienes o tienen que… ",
          },
        ],
      },

    listadoCompletarP53: [
          {
          listado: ["You are supposed to eat healthily"],
          textoA: "1. Respect elderly people (We)",
          textoD: "",
          tamano: "49",
        },
        {
          listado: ["You are supposed to eat healthily"],
          textoA: "2. Eat healthily (You)",
          textoD: "",
          tamano: "42",
        },
        {
          listado: ["The train is supposed to arrive at 11am, why is it so late?"],
          textoA: "3. Arrive at 11am, why is it so late? (The train)",
          textoD: "",
          tamano: "72.2",
        },
        {
          listado: ["I’m going to wash my bike now. I was supposed to wash it yesterday, but I didn’t want to"],
          textoA: "4. I have to give the bike back to Elena. It is dirty. Wash it (I)",
          textoD: "",
          tamano: "100",
        },
        {
          listado: ["Where is Hariette? She was supposed to be here an hour ago"],
          textoA: "5. Where is Hariette? It is late.  Be here (She",
          textoD: "",
          tamano: "74",
        },
      ],
    };
  },
};
</script>

<style>
</style>