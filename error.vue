<template>
    <div class="my-7 max-w-sm mx-auto text-center card">
        <p class="mb-7 text-6xl font-bold">{{ error.statusCode }}</p>
        <p class="mb-7 text-4xl">Ooops.</p>
        <p class="mb-7">{{ error.message }}</p>
        <button class="btn mb-7" @click="handleError">Go Home...</button>
    </div>
</template>

<script setup>

defineProps({
    error: Object
})
const handleError = () => clearError({ redirect: '/' })
</script>


<style scoped></style>