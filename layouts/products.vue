<template>
  <div>
    <header class="shadow-sm bg-white ">
      <nav class="container mx-auto p-4">
        <NuxtLink to="/products" class="font-bold">Nuxt App Merch</NuxtLink>
      </nav>
    </header>

    <div class="container mx-auto p-4 ">
      <slot />
    </div>

    <footer class="container mx-auto p-4 flex justify-berween border-t-2">
      <ul class=" flex gap-4 items-center">
        <li>
          <NuxtLink to="/">Home</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/about">About</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/products" class="btn">Products</NuxtLink>
        </li>
      </ul>
    </footer>
  </div>
</template>

<script setup>

</script>

<style scoped>
.router-link-exact-active {
  color: tomato;
}

nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

ul {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 16px;
  list-style: none;
  font-size: 16px;
  line-height: 1.2;
}
</style>