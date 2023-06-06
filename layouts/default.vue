<template>
  <div>
    <header class="shadow-sm bg-white ">
      <nav class="flex items-center justify-between contsiner mx-auto p-4">
        <NuxtLink to="/" class="font-bold ">Nuxt App</NuxtLink>
        <ul class=" flex items-center justify-center gap-4 text-base font-semibold">
          <li>
            <NuxtLink to="/" >Home</NuxtLink>
          </li>
          <li>
            <NuxtLink to="/about" >About</NuxtLink>
          </li>
          <li>
            <NuxtLink to="/products" class="btn">Products</NuxtLink>
          </li>
        </ul>
      </nav>
    </header>

    <div class="container mx-auto p-4">
      <slot />
    </div>
  </div>
</template>

<style scoped>
.router-link-exact-active {
  color: tomato;
  background: transparent;
  padding: 6px 12px;
  border: 1px solid tomato;
  border-radius: 10px;
}
</style>