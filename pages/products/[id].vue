 <template>
    <div>
 <p>Products details for {{ id }}</p>
 <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Qui, nulla!</p>
    </div>
 </template>
 
 <script setup>
 const { id } = useRoute().params

 definePageMeta({
  layout: 'products'
})
 </script>
 
 <style  scoped>
 
 </style>