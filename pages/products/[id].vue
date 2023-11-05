<template>
  <div>
    <p>the id is {{ id }}</p>
  </div>
</template>

<script setup>
const { id } = useRoute().params
</script>

<style   scoped>

</style>