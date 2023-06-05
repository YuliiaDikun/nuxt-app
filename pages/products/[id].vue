 <template>
    <div>
 <p>Products details for {{ id }}</p>
 <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Qui, nulla!</p>
    </div>
 </template>
 
 <script setup>
 const { id } = useRoute().params
 </script>
 
 <style  scoped>
 
 </style>