<template>
    <!-- <button @click="isListComp = !isListComp">
        <span v-if="isListComp">Table</span>
        <span v-else>List</span>
    </button> -->
    <br>
    <span>Megjelenités táblázatban: </span><input type="checkbox" @change="isListComp = !isListComp">

    <book-list @nevKuldes="adatFogado" v-if="isListComp" :bookList="bookList" />
    <book-table v-if="!isListComp" :bookList="bookList" />


    <div v-for="">

    </div>

</template>

<script setup>
import { ref } from 'vue';
import books from '../bookdata'
import BookTable from '../components/BookTable.vue';
import BookList from '../components/BookList.vue';


let bookList = ref([])
let isListComp = ref(true);
bookList.value = books

const nev = ref("")

const adatFogado = (par) => {
    console.log(par);
    nev.value = par
}


</script>