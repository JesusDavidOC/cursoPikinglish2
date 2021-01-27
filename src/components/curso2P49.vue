<template>
  <b-container fluid>
    <b-row>
      <b-col></b-col>
      <b-col sm="auto">
        <h3 class="titulo">MAY</h3>
      </b-col>
      <b-col></b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="auto">
        <p class="parrafo">
          <span class="colorLetraRojo">Negación:</span> MAY NOT
        </p>
        <p class="parrafo">
          <span class="colorLetraRojo">Significado:</span> poder, puede que y
          tener permiso.
        </p>
        <p class="parrafo"><span class="colorLetraRojo">Uso:</span></p>
        <p class="parrafo">1.Para ofrecer ayuda o para pedir permiso</p>
        <b-row>
          <b-col sm="1"></b-col>
          <b-col sm="auto">
            <p class="parrafo">
              Example:-
              <span class="colorLetraRojo">may</span> I help you?
            </p>
          </b-col>
        </b-row>
        <p class="parrafo">
          2. Para expresar probabilidad y es muy parecido al MIGHT.
        </p>
        <b-row>
          <b-col sm="1"></b-col>
          <b-col sm="auto">
            <p class="parrafo">
              Example: -She
              <span class="colorLetraRojo">may</span> test us tomorrow
            </p>
          </b-col>
        </b-row>
        <p class="parrafo">3. Para prohibiciones y autorizaciones.</p>
        <b-row>
          <b-col sm="1"></b-col>
          <b-col sm="auto">
            <p class="parrafo">
              Example: -you
              <span class="colorLetraRojo">may</span> not turn the volume up at
              night
            </p>
          </b-col>
        </b-row>

        <p class="parrafo">4. Para prohibiciones y autorizaciones.</p>
        <b-row>
          <b-col sm="1"></b-col>
          <b-col sm="auto">
            <p class="parrafo">
              Example: -I
              <span class="colorLetraRojo">may</span> be poor but I enjoy what I
              have.
            </p>
            <p class="parrafo">
              -She
              <span class="colorLetraRojo">may</span> not come to your birthday</p>
              <p class="parrafo">party but she will surely call you.</p>

          </b-col>
        </b-row>

        <p class="parrafo">
          5. Es casi igual que <span class="colorLetraRojo">Might</span> en
          realidad, pero se usa más en un lenguaje
        </p>
        <p class="parrafo">
          académico sobre las características o comportamiento de algo.
        </p>

        <b-row>
          <b-col sm="1"></b-col>
          <b-col sm="auto">
            <p class="parrafo">
              Example: -He
              <span class="colorLetraRojo">may</span> lose his job.
            </p>
            <p class="parrafo">
              -It <span class="colorLetraRojo">may</span> have a slice of bread
              and spread some jam through it.
            </p>
          </b-col>
        </b-row>
        <p class="parrafo">6. Para concederle el permiso a alguien</p>
        <b-row>
          <b-col sm="1"></b-col>
          <b-col sm="auto">
            <p class="parrafo">
              Example: -You
              <span class="colorLetraRojo">may</span> call me by my name
            </p>
            <p class="parrafo">
              -You <span class="colorLetraRojo">may</span> have a slice of bread
              and spread some jam through it
            </p>
          </b-col>
        </b-row>
      </b-col>
    </b-row>
    <b-row>
      <b-col sm="auto">
        <h3 class="subTitulo">PRACTICE. Fill out the gaps with May.</h3>
      </b-col>
    </b-row>

    <b-row>
      <b-col sm="1"></b-col>
      <b-col sm="11">
        <b-row
          v-for="(item, index) in listadoCompletarP49"
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
import inputChecked from "./inputChecked";
export default {
  components: {
    inputChecked,
  },
  data() {
    return {
      listadoCompletarP49: [
          {
          listado: ["May"],
          textoA: "1.",
          textoD: " I sit down? ",
          tamano: "20",
        },
        {
          listado: ["may"],
          textoA: "2. You",
          textoD: "choose what you like best ? ",
          tamano: "34",
        },
        {
          listado: ["may"],
          textoA: "3. You",
          textoD: "choose what you like best ? ",
          tamano: "34",
        },
        {
          listado: ["may"],
          textoA: "4. I don’t know how long we´ll stay at that hotel but we",
          textoD: "stay there a night or two.",
          tamano: "63.8",
        },
        {
          listado: ["May"],
          textoA: "5.",
          textoD: " I come in",
          tamano: "18.8",
        },
        {
          listado: ["may"],
          textoA: "6. We",
          textoD: " be friends but you don’t have the right to talk to me like that!",
          tamano: "55",
        },
      ],
    };
  },
};
</script>

<style>
</style>