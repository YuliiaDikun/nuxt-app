 <template>
    <div>
<p>{{ product.title }}</p>
<p>Price: {{ product.price }}</p>
<p>Product ID: {{ product.id }}</p>
    </div>
 </template>
 
 <script setup>
 const { id } = useRoute().params
const uri = `https://fakestoreapi.com/products/${id}`;

const {data: product} = await useFetch(uri, {key: id});

 definePageMeta({
  layout: 'products'
})
 </script>
 
 <style  scoped>
 
 </style>