<script setup>
import { ref } from 'vue';
let peoples = ['Alex','John','Rock','Tony']

</script>

<template>
    <p v-for="(person,index) in peoples" :key = "index">{{ person }}</p>
</template>