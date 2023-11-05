<template>
  <div>
    <header>
      <nav>
        <NuxtLink to="/products">Nuxt App | Merch</NuxtLink>
      </nav>
    </header>

    <!-- Output the page content -->
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

<style scoped>
header {
  background-color: #ccc;
  padding: 1rem;
}
.router-link-exact-active {
  color: #12b488;
}
</style>
