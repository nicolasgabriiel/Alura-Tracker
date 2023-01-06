<template>
  <main class="columns is-gapless is-multiline">
    
    <div class="column is-one-quarter">
      <BarraLateral/>
    </div><!--coluna 1-->
   
    <div class="column is-three-quarter">
      <Formulario @aoSalvarTarefa="salvarTarefa"/> 
      <div class="lista">
            <Tarefa v-for="(tarefa, index) in tarefas" :key="index" :tarefa="tarefa"/>
        </div>
    </div><!--coluna 2-->
  
  </main><!--corpo principal-->
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import BarraLateral from '../src/components/BarraLateral.vue'
import Formulario from '../src/components/Formulario.vue'
import  Tarefa  from './components/Tarefa.vue'
import ITarefa from './interfaces/ITarefa';

export default defineComponent({
  name: 'App',
  emits:['aoSalvarTarefa'] ,
  components: {
    BarraLateral,
    Formulario,
    Tarefa,
  },
  data(){
        return{
            tarefas: [] as ITarefa[]
        }
    },
    methods: {
      salvarTarefa(tarefa: ITarefa){
        this.tarefas.push(tarefa)
      }
    }
});
</script>


<style scoped>
.lista{
  padding: 1.25rem;
}

</style>
