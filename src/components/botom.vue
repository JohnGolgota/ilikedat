<template>
    <button @click="increment">
        +
    </button>
    <div>
        {{ count }}
    </div>
    <button @click="decrement">
        -
    </button>
</template>
<script setup lang="ts">
import { ref } from 'vue';
const count = ref(0)
const increment = () => count.value++
const decrement = () => count.value--
</script>
<style scoped>
button {
    background-color: #fff;
    border: 1px solid #999;
    border-radius: 3px;
    color: #666;
    font-size: 18px;
    padding: 5px 10px;
}

div {
    color: #666;
    font-size: 24px;
    padding: 5px 10px;
}
</style>