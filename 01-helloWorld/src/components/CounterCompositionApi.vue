<script setup>
//aki se utiliza la porperty setup del script
    import { ref } from 'vue';
    let count = ref(0)
    const addCounter= () => {
        count.value++
        console.log(count)
    }

</script>



<template>
    <div>
        
        <button @click="addCounter">ADD</button>
        <h3>{{ count }}</h3>
    </div>
</template>


<style scoped>


</style>