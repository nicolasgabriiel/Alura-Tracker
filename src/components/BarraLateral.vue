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
header{
    background: #0d3b66;
    width: 100%;
    height: 100vh;
    padding: 1rem;
}
@media only screen and (max-width: 768px){
    header{
        padding: 2.5rem;
        height: auto;
    }
}
</style>