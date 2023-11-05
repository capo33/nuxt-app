<template>
  <div>
    <div class="grid grid-cols-4 gap-5">
      <div v-for="p in products">
        <ProductCard :product="p"/>
      </div>
    </div>
  </div>
</template>

<script setup>
definePageMeta({
  layout: "products",
});
const { data: products } = await useFetch("https://fakestoreapi.com/products");

// one way to override metadata
useHead({
  title: "Products",
  meta: [
    {
      name: "description",
      content: "This is the products page",
    },
  ],
});
</script>

<style scoped></style>
