<script setup>
import {ref} from 'vue'
let input_text=ref('')
let agree=ref(false)
let country=ref('Facil')

</script>

<template>
<form>
    <div>
   <input type="text" name="from_1" id="1" v-model="input_text"/>
    </div>
   <input type="checkbox" v-model="agree"/> Acepto los terminos y condiciones
   <select v-model="country">
    <option >Facil</option>
    <option >Medio</option>
    <option >Dificil</option>
   </select>

</form>
<h2>{{ input_text }}</h2>


</template>

<style scoped>
</style>