<template>
  <div>
    <b-container fluid>
      <b-row>
        <b-col></b-col>
        <b-col sm="auto">
          <h3 class="titulo">THE USE OF ING </h3>
        </b-col>
        <b-col></b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            En muchos casos el uso del gerundio ING en inglés no significa que la terminación sea ANDO o ENDO
            en español, sino que simplemente es una cuestión gramatical y no literal. Veamos en detalle el uso del ING
            en inglés.  
          </h3>
        </b-col>
      </b-row>
      <br><br>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="10">
          <tablaTC :cuestionario="tabla3P7" />
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="11">
          <h3 class="subTitulo">
            ING TIEMPO PROGRESIVO
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            After IS, AM, ARE, WAS, WERE, BE, BEEN
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3>
            <b>1. </b> I <span class="colorLetraRojo"> am</span> sit<span class="colorLetraRojo">ting</span> here in the living room <br><br>
            <b>2. </b>	She <span class="colorLetraRojo">  is</span> stand<span class="colorLetraRojo">ing </span> <br><br>
            <b>3. </b>	He <span class="colorLetraRojo">is</span>  wonder<span class="colorLetraRojo">ing</span> what to do <br><br>
            <b>4. </b>	It <span class="colorLetraRojo"> is </span>  rain<span class="colorLetraRojo">ing</span> cats and dogs <br><br>
            <b>5. </b>	You <span class="colorLetraRojo"> are</span> improv<span class="colorLetraRojo">ing</span> your speaking skill <br><br>
            <b>6. </b>	We <span class="colorLetraRojo">are</span>  ly <span class="colorLetraRojo">ing</span> down on the grass looking up at the stars  <br><br>
            <b>7. </b>	They <span class="colorLetraRojo">are</span>  discuss<span class="colorLetraRojo">ing</span> the rules of the house with their children <br><br>
            <b>8. </b>	I <span class="colorLetraRojo"> was</span> think<span class="colorLetraRojo">ing</span> about what I am doing next <br><br>
            <b>9. </b>	Those people <span class="colorLetraRojo">were</span>  try<span class="colorLetraRojo">ing </span>to break into the office. <br><br>
            <b>10. </b>	I will <span class="colorLetraRojo"> be</span> work<span class="colorLetraRojo">ing</span> all day tomorrow <br><br>
            <b>11.</b>	I have <span class="colorLetraRojo">been</span>  practic<span class="colorLetraRojo">ing</span> Spanish 
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="11">
          <h3 class="subTitulo">
            ING CUANDO UN VERBO ES USADO COMO SUJETO.
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            El verbo es el sujeto de la oración y es tercera persona del singular.
          </h3>
        </b-col>
      </b-row>
      <br>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3>
            <b>1. </b> <span class="colorLetraRojo">Eating</span> healthy helps your digestive system work better <br><br>
            <b>2. </b> Speak<span class="colorLetraRojo">ing</span> English gives you more opportunities to get a job. <br><br>
            <b>3. </b> I don’t think that learn<span class="colorLetraRojo">ing</span> English is difficult <br><br>
            <b>4. </b> Is do<span class="colorLetraRojo">ing</span> sports in the morning better than at night? <br><br>
            <b>5. </b> Does talk<span class="colorLetraRojo">ing</span> to her make you feel better when you are sad? <br><br>
            <b>6. </b> Driv<span class="colorLetraRojo">ing</span> fast when it is raining might cause an accident
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="11">
          <h3 class="subTitulo">
            ING DESPUÉS DE UNA PREPOSICIÓN
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            In, at, after, before, on, of, off, with, for, by, out, about, to, up, down, over, though, across, into, onto, inside.
          </h3>
        </b-col>
      </b-row>
      <br>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3>
            <b>IN: </b> I am interested <span class="colorLetraRojo">in</span> learn<span class="colorLetraRojo">ing</span> English <br><br>
            <b>AT: </b>  I am good <span class="colorLetraRojo">at</span> cook <span class="colorLetraRojo">ing</span>  <br> <br>
            <b>AFTER:</b> <span class="colorLetraRojo">After</span> hav<span class="colorLetraRojo">ing</span> said that, he left <br><br>
            <b>BEFORE:</b>  You have to take off your shoes <span class="colorLetraRojo">before</span> enter<span class="colorLetraRojo">ing</span> the room. <br><br>
            <b> ON:</b> I need to focus <span class="colorLetraRojo">on</span> finish<span class="colorLetraRojo">ing</span> this project.  <br><br>
            <b>OF:</b>  here we state 10 ways of improv<span class="colorLetraRojo">ing</span> your English. <br><br>
            <b>OFF:</b>  I can ́t put <span class="colorLetraRojo"> off</span> go<span class="colorLetraRojo">ing</span> to the dentist today. <br><br>
            <b>WITH:</b>  I am fed up <span class="colorLetraRojo">with</span> working on Sundays. <br><br>
            <b>FOR:</b>  I am here to thank you <span class="colorLetraRojo">for</span> help<span class="colorLetraRojo">ing</span> me take care of my son. <br><br>
            <b>BY:</b>  You can lose some pounds <span class="colorletraRojo">by</span> eat <span class="colorLetraRojo">ing</span> more vegetables and fruits. <br><br>
            <b>ABOUT:</b>  I am always thinking <span class="colorLetraRojo">about </span> travel<span class="colorLetraRojo">ing</span> in my car. <br><br>
            <b>TO:</b> I am looking forward <span class="colorLetraRojo">to</span>  paint<span class="colorLetraRojo">ing</span> my house
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="11">
          <h3 class="subTitulo">
            ING EN VERBOS CONVERTIDOS EN ADJETIVOS.
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            Cuando decimos para que sirve algo el verbo se convierte en un adjetivo.
          </h3>
        </b-col>
      </b-row>
      <br>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3>
            <b>1. </b> Zapatos para correr: <span class="colorLetraRojo">Running</span> <b>shoes</b> <br><br>
            <b>2. </b> Tabla para cortar: <span class="colorLetraRojo">Cutting</span> <b>board</b> <br><br>
            <b>3. </b> Licencia para conducir: <span class="colorLetraRojo">Driving</span> <b>license</b> <br><br>
            <b>4. </b> Permiso para trabajar: <span class="colorLetraRojo">Working</span> <b>permission</b> <br><br>
            <b>5. </b> Lote para parquear: <span class="colorLetraRojo"> Parking</span> <b>lot</b> <br><br>
            <b>6. </b> Carro para las compras: <span class="colorLetraRojo">Shopping</span> <b>cart</b>
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="11">
          <h3 class="subTitulo">
            ING ACTIVIDADES DE OCIO CON EL VERBO GO
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            Si la actividad lleva un objeto no aplica esta estructura. Por ejemplo: Ir a estudiar <span class="colorLetraRojo">inglés.</span> Ir a tomar
            <span class="colorLetraRojo">cerveza,</span> ir a escuchar <span class="colorLetraRojo">música</span> etc.
          </h3>
        </b-col>
      </b-row>
      <br>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3>
            <b>1. </b> Go shopp<span class="colorLetraRojo">ing</span>: Ir de compras. I think I ́ll go shopping later <br><br>
            <b>2. </b> Go runn<span class="colorLetraRojo">ing</span>: Ir a correr. I have not gone running in a while <br><br>
            <b>3. </b> Go danc<span class="colorLetraRojo">ing</span>: Ir a bailar. Would you like to go dancing? <br><br>
            <b>4. </b> Go swimm<span class="colorLetraRojo">ing</span>: Ir a nadar. I went swimming last week <br><br>
            <b>5. </b> Go fish<span class="colorLetraRojo">ing</span>: Ir de pesca. It sounds like a great idea to go fishing this week. <br><br>
            <b>6. </b> Go walk<span class="colorLetraRojo">ing</span>: Ir a caminar. The most I enjoy doing is to go walking down the beach <br><br>
            <b>7. </b> Go climb<span class="colorLetraRojo">ing</span>: Ir a escalar. I am very excited about going rock climbing tomorrow <br><br>
            <b>8. </b> Go camp<span class="colorLetraRojo">ing</span>: Ir a campar. Have you ever gone camping? <br><br>
            <b>9. </b> Go horseback rid<span class="colorLetraRojo">ing</span>: Ir a montar caballo. Who wants to go horseback riding? <br><br>
            <b>10. </b> Go sightsee<span class="colorLetraRojo">ing</span>: Ir a conocer la ciudad. We may go sightseeing later.
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="11">
          <h3 class="subTitulo">
            ING DESPUÉS DE WHEN Y WHILE
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3>
            <b>1. </b> Don´t talk on the phone when driv<span class="colorLetraRojo">ing</span> (When you are driving) <br><br>
            <b>2. </b> It is important to keep the gate locked while living here
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="11">
          <h3 class="subTitulo">
            ING DESPUÉS DE ALGUNOS VERBOS
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            <b>FIRST GROUP:</b> Verbs of <b>liking and disliking:</b> 
          </h3>
        </b-col>
      </b-row>
      <br>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            Detest <b> -</b> Dislike <b>- </b> Enjoy <b>- </b>Fancy <b>- </b> Hate <b>- </b>Like <b>- </b>Love
          </h3>
        </b-col>
      </b-row>
      <br>
      <br>
      
      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3>
            <b>1. </b> My mother detests giv<span class="colorLetraRojo">ing</span> you an order twice <br><br>
            <b>2. </b> I dislike driv<span class="colorLetraRojo">ing</span> by night <br><br>
            <b>3. </b> I enjoy ly<span class="colorLetraRojo">ing</span> down on the grass <br><br>
            <b>4. </b> I am hungry. I fancy eat<span class="colorLetraRojo">ing</span> fried chicken <br><br>
            <b>5. </b> I hate work<span class="colorLetraRojo">ing</span> with her <br><br>
            <b>6. </b> I like cook<span class="colorLetraRojo">ing</span> <br><br>
            <b>7. </b> I love runn<span class="colorLetraRojo">ing</span> in the rain
          </h3>
        </b-col>
      </b-row>
      <br>

      <b-row>
        <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            <b> SECOND GROUP:</b> after the verb “mind
          </h3>
        </b-col>
      </b-row>
      <br>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3>
            <b>1. </b> Would you mind opening the door, it is too hot in here. <br><br>
            <b>2. </b> I don’t mind traveling by bus.
          </h3>
        </b-col>
      </b-row>
      <br>

      <b-row>
        <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            <b>THIRD GROUP:</b> Verbs of saying and thinking:
          </h3>
        </b-col>
      </b-row>
      <br>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            Admit <b>-</b> Consider <b>-</b> Deny <b>-</b> Imagine <b>-</b> Remember <b>-</b> Suggest
          </h3>
        </b-col>
      </b-row>
      <br><br>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3>
            <b>1. </b> She admitted <span class="colorLetraRojo">taking </span>the car without permission <br><br>
            <b>2. </b> We should consider <span class="colorLetraRojo">buying</span> the blue car as soon as possible <br><br>
            <b>3. </b> You can ́t deny <span class="colorLetraRojo">cloving</span> her <br><br>
            <b>4. </b> I imagine myself <span class="colorLetraRojo">living</span> in a cabin <br><br>
            <b>5. </b> I remember <span class="colorLetraRojo">being</span> in the army in 2007.
          </h3>
        </b-col>
      </b-row>
      <br>

      <b-row>
        <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            <b>FOURTH GROUP:</b> Others verbs
          </h3>
        </b-col>
      </b-row>
      <br>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            Avoid <b>-</b> Begin <b>-</b> Finish <b>-</b> Keep <b>-</b> Miss <b>-</b> Practice <b>-</b> Risk <b>-</b> Start <b>-</b> Stop
          </h3>
        </b-col>
        </b-row>
        <br><br>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3>
            <b>1. </b> How can I avoid speak<span class="colorLetraRojo">ing</span> to them? <br><br>
            <b>2. </b> I began eat<span class="colorLetraRojo">ing</span> less and healthier since I had a heart attack <br><br>
            <b>3. </b>I have to finish print<span class="colorLetraRojo">ing</span> this book by the end of this month <br><br>
            <b>4. </b> we can ́t keep act<span class="colorLetraRojo">ing</span> as if nothing had happened. <br><br>
            <b>5. </b> You have no idea how much I miss talk<span class="colorLetraRojo">ing</span> to you. <br><br>
            <b>6. </b> You need to practice swimming in the pool before swimm<span class="colorLetraRojo">ing</span> in a river. <br><br>
            <b>7.</b> I can ́t risk los<span class="colorLetraRojo">ing</span> job <br> <br>
            <b>8. </b> I started learn<span class="colorLetraRojo">ing</span> English when I was 22 <br><br>
            <b>9. </b> Life never stops teach<span class="colorLetraRojo">ing</span> you new things
          </h3>
        </b-col>
      </b-row>
      <br>

      <b-row>
        <b-col sm="auto"><i class="fa fa-diamond fuenteDiamond"></i></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            <b>FIFTH GROUP: </b> VERBOS DE LOS SENTIDOS Y OTROS. Estructura: verbo + objeto + verbo + ing
          </h3>
        </b-col>
      </b-row>
      <br>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3 class="parrafoIC">
            see <b>-</b> hear <b>-</b> listen to <b>-</b> smell <b>-</b> watch <b>-</b> catch <b>-</b> find <b>-</b> imagine <b>-</b> leave <b>-</b> prevent <b>-</b> stop
          </h3>
        </b-col>
      </b-row>
      <br><br>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3>
            <b>1.</b> We saw everybody ru<span class="colorLetraRojo">nning</span> ing away <br><br>
            <b>2.</b> I caught someone try<span class="colorLetraRojo">ing</span> to break into my house. <br><br>
            <b>3.</b> We couldn’t prevent them ge<span class="colorLetraRojo">tting</span> away. <br><br>
            <b>4.</b> I heard Johnny talk<span class="colorLetraRojo">ing</span> about me <br><br>
            <b>5.</b> I listened to the band play<span class="colorLetraRojo">ing</span> at the restaurant as I ate <br><br>
            <b>6.</b> I smelled the carcass rott<span class="colorLetraRojo">ing</span> in the hot sun <br><br>
            <b>7.</b> I found him drink<span class="colorLetraRojo">ing</span> in the bar <br><br>
            <b>8.</b> I can ́t imagine myself liv<span class="colorLetraRojo">ing</span> in a big city <br><br>
            <b>9.</b> Have you ever seen your teacher fight<span class="colorLetraRojo">ing?</span> <br><br>
            <b>10.</b> No one is going to stop me travel<span class="colorLetraRojo">ing</span><br><br>
            <b>11.</b> My parents left me driv<span class="colorLetraRojo">ing</span> back home from the gas station
          </h3>
        </b-col>
      </b-row>
      
      <b-row>
        <b-col sm="auto"></b-col>
        <b-col sm="11">
          <h3 class="subTitulo">
            ING DESPUÉS DE ESTAS EXPRESIONES
          </h3>
        </b-col>
      </b-row>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3>
            <b>I can´t help:</b> no puedo dejar de. <br><br>
            <b>It is worth:</b> vale la pena. <br><br>
            <b>Have difficulty:</b> tener dificultades. <br><br>
            <b>There is no point:</b> no tener sentido.  <br><br>
            <b>Spend time:</b> pasar tiempo.  <br><br>
            <b>I can´t bear / stand :</b> no puedo tolerar o soportar. <br><br>
            <b>It is no use / it is no good:</b> de nada sirve. <br> <br>
            <b>Have trouble:</b> tener problemás.  <br> <br>
            <b>It is a waste of money or time:</b> es una Perdida de dinero o tiempo.  <br><br>
            <b>Waste time:</b> desperdiciar el tiempo. 
          </h3>
        </b-col>
      </b-row>
      <br><br>

      <b-row>
        <b-col sm="1"></b-col>
        <b-col sm="11">
          <h3>
            <b>1.</b> There's nothing you can do about the sitúation, so <b>it's no use</b> worry<span class="colorLetraRojo">ing</span> about it. <br><br>
            <b>2. It's no good</b> try<span class="colorLetraRojo">ing</span> to persuade me. You won't succeed.<br><br>
            <b>3. There's no point in</b> hav<span class="colorLetraRojo">ing</span> a car if you never use it. <br><br>
            <b>4. There was no point in</b> wait<span class="colorLetraRojo">ing</span> any longer, so we went. <br><br>
            <b>5.</b> I live only a short walk from here, so <b>it's not worth</b> tak<span class="colorLetraRojo">ing</span> a taxi. <br><br>
            <b>6.</b> Our flight was very early in the morning, so <b>it wasn't worth</b> go<span class="colorLetraRojo">ing</span> to bed<br><br>
            <b>7.</b> What was the film like? Was it <b>worth see</b><span class="colorLetraRojo">ing</span> ? <br><br>
            <b>8.</b> Thieves broke into the house but didn't take anything. There was nothing <b>worth steal</b><span class="colorLetraRojo">ing</span>. <br><br>
            <b>9.</b> I had no <b>difficulty</b> find<span class="colorLetraRojo">ing</span>a place to live. <br><br>
            <b>10.</b> Did you have any <b>difficulty</b> gett<span class="colorLetraRojo">ing</span> a job?<br><br>
            <b>11.</b> People often have <b>difficulty</b> read<span class="colorLetraRojo">ing</span> my writing. <br><br>
            <b>12.</b> I had no <b>trouble</b> find<span class="colorLetraRojo">ing</span> a place to live. <br><br>
            <b>13.</b> It was a <b>waste of time</b> read<span class="colorLetraRojo">ing</span> that book. It was rubbish. <br><br>
            <b>14.</b> It's a <b>waste of money</b> buy<span class="colorLetraRojo">ing</span> things you don't need. <br><br>
            <b>15.</b> He <b>spent</b> hours try<span class="colorLetraRojo">ing</span> to repair the clock. <br><br>
            <b>16.</b> I <b>wasted</b> a lot of time think<span class="colorLetraRojo">ing</span>  about the problem.
          </h3>
        </b-col>
      </b-row>
      
    </b-container>
  </div>
</template>

<script>
import posiblesRespuestasTabla from "./posiblesRespuestasTabla";
import opcionMultiple from "./opcionMultiple";
import listaIndex from "./listaIndex";
import inputChecked from "./inputChecked";
import tablaTC from "./tablaTraduccionCodigos";
import inputCheckedE from "./inputCEnriquecido";
import InputChecked from "./inputChecked.vue";
export default {
  components: {
    tablaTC,
    inputChecked,
    listaIndex,
    opcionMultiple,
    posiblesRespuestasTabla,
    inputCheckedE,
  },
  data(){
    return{
      tabla3P7:{
        fields:[ 
          { key: "html1", thClass:"noHead"},
          { key: "html2", thClass:"noHead"},
          { key: "html3", thClass:"noHead"},
        ],
        items:[
          {
            html1:"Tiempo progresivo",
            html2:"After IS, AM, ARE, WAS, WERE, BE, BEEN",
            html3:"I am <span class='colorLetraRojo'>working</span>"
          },
          {
            html1:"Cuando un verbo es usado como sujeto.",
            html2:"",
            html3:"<span class='colorLetraRojo'> Eating </span> healthy helps your digestive system work better"
          },
          {
            html1:"Después de una preposición",
            html2:"In, at, after, before, on, of, with, for, by, with, out, about, to, up,down, over, though, across,while etc.",
            html3:"After <span class='colorLetraRojo'>eating</span>, wash your hands"
          },
          {
            html1:"Adjetivos de opinión.",
            html2:"Surprise-surprising",
            html3:"That was a <span class='colorLetraRojo'>surprising </span>moment"
          },
          {
            html1:"Cuando un verbo se convierte en adjetivo Describe para que es algo.",
            html2:"Love-loving Drive-driving",
            html3:"I always remember the<span class='colorLetraRojo'> loving </span >moments we spent together. <br><br> I am taking <span class='colorLetraRojo'> driving </span> lessons <span class='letraColorRojo'> running </span> shoes."
          },
          {
            html1:"Después del verbo GO cuando se refiere a una actividad",
            html2:"Go shopping <br> Go running <br>Go dancing <br>Go swimming<br>Go fishing ",
            html3:"One of my favorite things to do is to go <span class='colorLetraRojo'>running</span> in the rain."
          },
          {
            html1:"Después de estos verbos",
            html2:"love, like, hate, stop, start, fancy, deny, avoid, postpone, remember, regret, propose, quit, mind, keep, enjoy, finish, admit, miss, risk, consider.",
            html3:"-I don’t mind <span class='colorLetraRojo'> staying </span> home - I regret going out last night"
          },
          {
            html1:"Después de estas expresiones",
            html2:"Can ́t help, can ́t stand, can ́t bear, it is worth, it is use, I have difficulty",
            html3:"I can’t help <span class='colorLetraRojo'> thinking  </span> about that problem.<br><br> I have difficulty <span class='colorLetraRojo'>understanding</span> Spanish"
          },
          {
            html1:"Estructura de verbo más objeto más verbo",
            html2:" - verbs of the senses: <br><br> see hear listen to smell watch catch find imagine leave prevent stop",
            html3:"We saw everybody <span class='colorLetraRojo'> running </span> away <br><br> -I caught someone <span class='colorLetraRojo'> trying  </span>to break in to my house.<br><br> -We couldn’t prevent them <span class='colorLetraRojo'> getting  </span>away."
          },
          {
            html1:"Despúes de When y While",
            html2:"En ingles se usa el verbo con ing despues de When y While",
            html3:"Dont talk on the phone when driving "
          },
        ]
      }
    }
  }
}
</script>
