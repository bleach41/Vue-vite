<script setup>
import CounterCompositionApi from './components/CounterCompositionApi.vue';
import CounterOptionApi from './components/CounterOptionApi.vue';
import ExampleBind from './components/ExampleBind.vue';
import ExampleFor from './components/ExampleFor.vue';
import ExampleSelective from './components/ExampleSelective.vue';
import ModelForm from './components/ModelForm.vue';
import PostConteiner from './components/PostConteiner.vue'

import { ref } from 'vue';

const darkTheme = ref(false);

function toggleTheme() {
  darkTheme.value = !darkTheme.value;
  if (darkTheme.value) {
    document.documentElement.classList.add('dark-theme');
  } else {
    document.documentElement.classList.remove('dark-theme');
  }
}





</script>

<template>

    <div >
      <ModelForm/>
      <button @click="toggleTheme">Cambiar tema</button>
      <div :class="{ dark: darkTheme }">
        <CounterCompositionApi/>
        <ExampleBind/>
        <ExampleFor/>
        <h1>HOLA MUNDO</h1>
        <CounterOptionApi/>
        <ExampleSelective/>
        <PostConteiner />
      </div>
    </div>
  </template>




<style>

h1{

  filter: blur(5px);
  color: aqua;
}

h1:hover{
  filter: blur(0);
  cursor: pointer;
  scale: 1.05;
}
div{
  padding: 1px
}

.dark-theme {

  color:black;
  background-color: rgb(131, 135, 134);

}


</style>
