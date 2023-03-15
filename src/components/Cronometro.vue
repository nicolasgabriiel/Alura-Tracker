<template>
    <section>
        <strong>{{ tempoDecorrido }}</strong>
    </section>
</template>

<script lang="ts">
import { defineComponent, DefineComponent } from 'vue';
export default defineComponent({
    name:'Cronometro-vue',
    computed:{
        tempoDecorrido () : string{
            return new Date(this.tempoEmSegundos * 1000).toISOString().substr(11,8)
        }
    },
    props:{
        tempoEmSegundos:{
            type: Number,
            default: 0
        }
    }
})
</script>

<style></style>