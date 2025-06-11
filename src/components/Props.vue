<script setup>
    // const props = defineProps(['name','age'])

    // const props = defineProps({
    //     name: String,
    //     age: Number
    // })


    // IMP: Validator function used in define props- can be used for some basic authentication 

    const props = defineProps({
        name: {
            type: String,
            required: true,
            default: 'anonymous'
        },
        age: Number
    })
</script>

<template>
    <h1>{{ props.name }}</h1>
    <h1>{{ props.age }}</h1>
</template>