<template>
  <div>
    <h2>About</h2>
    <p>{{ data }}</p>
  </div>
</template>

<script setup>
const { data } = await useFetch("/api/test?name=capo", {
  method: "post",
  body: { age: 25 },
});
</script>

<style scoped></style>
