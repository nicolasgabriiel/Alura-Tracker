<template>
  <main class="columns is-gapless is-multiline">
    
    <div class="column is-one-quarter">
      <BarraLateral/>
    </div><!--coluna 1-->
   
    <div class="column is-three-quarter">
      <Formulario/> 
    </div><!--coluna 2-->
  
  </main><!--corpo principal-->
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import BarraLateral from '../src/components/BarraLateral.vue'
import Formulario from '../src/components/Formulario.vue'

export default defineComponent({
  name: 'App',
  components: {
    BarraLateral,
    Formulario
  }
});
</script>
