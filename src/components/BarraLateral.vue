<template>
  <header>
    <h1>
        <img src="../assets/logo.png">
    </h1>
  </header>

</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
    name:'Barra-Lateral'
})
</script>

<style scoped>
@media only screen and (max-width: 768px){
    header{
        padding: 2.5rem;
        height: auto;
    }
}
</style>