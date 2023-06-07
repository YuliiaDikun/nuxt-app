<template>
  
    <ul class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-5">
      <li v-for="product in products">
        <ProductCard :product="product"/>
      </li>
    </ul>
  
</template>

<script setup>
definePageMeta({
  layout: 'products'
})

const { data: products } = await useFetch('https://fakestoreapi.com/products')

useHead({
  title: 'Nuxt Merch Page',
      meta: [
        { name: 'description', content: 'Our shop merch' }
      ],
})
</script>

<style lang="scss" scoped></style>