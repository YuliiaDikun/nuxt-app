<template>
  <div>
    <header>
      <nav>
        <NuxtLink to="/products">Nuxt App Merch</NuxtLink>
      </nav>
    </header>

    <div>
      <slot />
    </div>

    <footer>
      <ul>
        <li>
          <NuxtLink to="/">Home</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/about">About</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/products">Products</NuxtLink>
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