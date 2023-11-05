<template>
  <div>
    <h2>About</h2>
    <p>Current currency: {{ data }}</p>
  </div>
</template>

<script setup>
const { data } = await useFetch("/api/currency/GBP");
</script>

<style scoped></style>
