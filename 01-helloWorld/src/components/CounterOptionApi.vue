<script >
    import { defineComponent } from 'vue';
    export default defineComponent({
        name: 'CounterOption',
        data(){
            let counter=0;
            return{counter}
        },
        methods: {
            addCounter(){
                this.counter++
            }
        }
    })

</script>



<template>
    <div>
        <h3>{{ counter }}</h3>
        <button @click="addCounter">Incrementar</button>
    </div>
</template>


<style scoped>


</style>