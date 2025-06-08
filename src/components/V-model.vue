<script setup>
    import { ref } from 'vue'
    const formData = ref({
        username: '',
        email:'',
        password:''
    })
</script>

<template>
    <form @submit.prevent> 
        <input type = "text" placeholder = "Enter your name" v-model="formData.username">
        <input type = "email" placeholder = "Enter your email" v-model="formData.email">
        <input type = "password" placeholder = "Enter your password" v-model="formData.password">
        <button type="submit">Submit</button>
    </form>
    <h1>
        {{ formData.username }} {{ ' ' }}
        {{ formData.email }} {{ ' ' }}
        {{ formData.password }}
    </h1>
</template>