<script setup>
import PostCard from './PostCard.vue';
import {ref} from 'vue'
const tarjs=ref([
    PostCard, PostCard, PostCard
])
</script>

<template>
    <div >
        <ul>
            <PostCard v-for="(tarj,index) in tarjs" v-bind::key="index">{{ tarj }}</PostCard>
        </ul>
    </div>
</template>


<style scoped>

</style>