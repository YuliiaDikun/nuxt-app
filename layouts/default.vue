<template>
    <div>
      <header>
        <nav>
          <NuxtLink to="/">Nuxt App</NuxtLink>
          <ul>
            <li><NuxtLink to="/">Home</NuxtLink></li>
            <li><NuxtLink to="/about">About</NuxtLink></li>
            <li><NuxtLink to="/products">Products</NuxtLink></li>
          </ul>
        </nav>
      </header>
  
     <div>
        <slot/>
     </div>
    </div>
  </template>

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