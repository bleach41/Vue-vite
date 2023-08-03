<script setup>
import {ref} from 'vue'
let c = ref('#ccc')
const handleClick=()=>{
    if (c.value==='#ccc'){
        c.value='#000'
    }
    else
    c.value='#ccc'   
}

</script>

<template>
<p v-bind:style="{color: c}">Texto de prueba</p>
<button @click="handleClick()">color</button>
</template>

<style scoped>

</style>