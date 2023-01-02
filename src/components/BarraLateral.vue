<!--Aqui vai o HTML-->
<template>
    <header>
        <h1>
            <img src="../assets/logo.png" alt="logo">
        </h1>
    </header>
</template>

<!--Aqui vai o TypeScript-->
<script lang="ts">

import { defineComponent } from 'vue';

export default defineComponent ({
    name: "BarraLateral"
} )

</script>

<!--Aqui vai o Css (o SCOPED é importante para o style funcionar apenas nesse componente)-->
<style scoped>
header{
    background-color: #0d3b66;
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