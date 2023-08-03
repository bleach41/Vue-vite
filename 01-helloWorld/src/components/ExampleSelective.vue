
<script setup>
//aki se utiliza la porperty setup del script
let age=50

</script>



<template>
    <div>
        <h2 v-show="age > 18">Eres mayor de edad</h2>
        <h2 v-show="age <=18">Eres menor de edad</h2>
    </div>
</template>


<style scoped>


</style>