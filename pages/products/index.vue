<template>
    <div>

        <ul class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-5">
            <li v-for="p in products">
                <NuxtLink :to="`/products/${p.id}`">
                    {{ p.title }}
                </NuxtLink>
            </li>
        </ul>

    </div>
</template>

<script setup>
definePageMeta({
    layout: 'products'
})

const { data: products } = await useFetch('https://fakestoreapi.com/products')


</script>

<style lang="scss" scoped></style>