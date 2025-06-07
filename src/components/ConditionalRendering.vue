<script setup>
    const isTrue = null
</script>

<template>
    <div>
        <p v-if="isTrue==true">This will show if isTrue is true.</p>
        <p v-else-if="isTrue==false">This will show if isTrue is not true.</p>
        <p v-else>This will show if isTrue is not a boolean.</p>
    </div>
</template>