<script setup>
import PostCard from './PostCard.vue'
</script>

<template>
    <div class="post-conteiner">
        
        <PostCard />
        <PostCard />
        <PostCard />
        <PostCard />
 </div>
</template>

<style scoped>

.pos-conteiner{

    width: 100%;
    display: flex;
    flex-wrap: wrap;
}
</style>