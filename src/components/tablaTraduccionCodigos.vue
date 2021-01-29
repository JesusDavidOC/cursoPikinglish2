<template>
<div class="overflow-auto maxh">
    <b-table id="cuestionario" small :fields="this.cuestionario.fields" :items="this.cuestionario.items" responsive="sm" :bordered="true">
        <template v-slot:cell(complejo1)="row" id="hola921">
            <inputChecked :resuelto="row.item.complejo1.resuelto" :esperado="row.item.complejo1.lista" :conTexto="true" :textoA="row.item.complejo1.textoA" :textoD="row.item.complejo1.textoD" :textoD2="row.item.complejo1.textoD2" :audio="row.item.complejo1.audio" :tamano="row.item.complejo1.tamano" />
        </template>
        <template v-slot:cell(complejo2)="row" id="hola7471">
            <inputChecked :resuelto="row.item.complejo2.resuelto" :esperado="row.item.complejo2.lista" :conTexto="true" :textoA="row.item.complejo2.textoA" :textoD="row.item.complejo2.textoD" :textoD2="row.item.complejo2.textoD2" :audio="row.item.complejo2.audio" :tamano="row.item.complejo2.tamano" />
        </template>

        <template v-slot:cell(complejo3)="row" id="hola7417">
            <inputChecked :resuelto="row.item.complejo3.resuelto" :esperado="row.item.complejo3.lista" :conTexto="true" :textoA="row.item.complejo3.textoA" :textoD="row.item.complejo3.textoD" :textoD2="row.item.complejo3.textoD2" :audio="row.item.complejo3.audio" :tamano="row.item.complejo3.tamano" />
        </template>

        <template v-slot:cell(complejo4)="row" id="hola7427737452">
            <inputChecked :resuelto="row.item.complejo4.resuelto" :esperado="row.item.complejo4.lista" :conTexto="true" :textoA="row.item.complejo4.textoA" :textoD="row.item.complejo4.textoD" :textoD2="row.item.complejo4.textoD2" :audio="row.item.complejo4.audio" :tamano="row.item.complejo4.tamano" />
        </template>

        <template v-slot:cell(complejo5)="row" id="hola737375375">
            <inputChecked :resuelto="row.item.complejo5.resuelto" :esperado="row.item.complejo5.lista" :conTexto="true" :textoA="row.item.complejo5.textoA" :textoD="row.item.complejo5.textoD" :textoD2="row.item.complejo5.textoD2" :audio="row.item.complejo5.audio" :tamano="row.item.complejo5.tamano" />
        </template>

        <template v-slot:cell(complejo21)="row" id="hola742742742">
            <inputCE :style="'width:' + row.item.complejo21.tamano + 'em;'" :object="row.item.complejo21" />
        </template>

        <template v-slot:cell(html1)="row" id="hola">
            <a v-html="row.item.html1"> {{ row.item.html1 }} </a>
        </template>

        <template v-slot:cell(html2)="row" id="hola2">
            <a v-html="row.item.html2"> {{ row.item.html2 }} </a>
        </template>

        <template v-slot:cell(html3)="row" id="hola3">
            <a v-html="row.item.html3"> {{ row.item.html3 }} </a>
        </template>

         <template v-slot:cell(complejoAudio1)="row" id="holaAudio">
            <audioComp :elemento=" row.item.complejoAudio1" />
        </template>

        <template v-slot:cell(complejoAudio2)="row" id="holaAudio2">
            <audioComp :elemento=" row.item.complejoAudio2" />
        </template>

        <template v-slot:cell(complejoAudio3)="row" id="holaAudio3">
            <audioComp :elemento=" row.item.complejoAudio3" />
        </template>
        <template v-slot:cell(complejoAudio4)="row" id="holaAudio4">
            <audioComp :elemento=" row.item.complejoAudio4" />
        </template>
        <template v-slot:cell(complejoAudio5)="row" id="holaAudio5">
            <audioComp :elemento=" row.item.complejoAudio5" />
        </template>
    </b-table>
</div>
</template>

<script>
import inputChecked from "./inputChecked";
import inputCE from "./inputCEnriquecido";
import audioComp from "./audioComp"

export default {
    components: {
        inputChecked,
        inputCE,
        audioComp,
    },
    props: {
        cuestionario: Object,
        espanolR: Boolean,
        inglesR: Boolean,
    },
    mounted() {},
};
</script>

<style scoped>
/deep/ td{
    font-size: 1.5em;
}

/deep/ td .ic{
    font-size: 0.7em !important;
}

.cuestionario{
    border-width: 0px;
}

/deep/ .table-bordered{
    border: 0px !important;
    width: 99.9%;
}

/deep/ th{
    font-size: 1.5em !important;    
    text-align: center;
}

/deep/ .noHead{
    font-size: 0em !important;
}

</style>
