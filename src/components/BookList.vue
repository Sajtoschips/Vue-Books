<template>
    <ul>
        <li v-for="(liItem) in bookList">{{ liItem.title }}</li>
    </ul>
    <label for="nev"></label>
    <input type="text" id="nev" v-model="name">
    <button @click="$emit('nevKuldes', name)">Elküld</button>
</template>

<script setup>
import { ref } from 'vue';

const name = ref("")

defineProps(["bookList"])

</script>