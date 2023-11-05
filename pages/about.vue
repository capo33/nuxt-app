<template>
  <div>
    <h2>About</h2>
    <p v-for="d in data">{{ d.code }}</p>
  </div>
</template>

<script setup>
const { data } = await useFetch("/api/test");
</script>

<style scoped></style>
