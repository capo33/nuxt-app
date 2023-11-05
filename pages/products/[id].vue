<template>
  <div>
    <p>the id is {{ id }}</p>
    <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quos modi repellat aut, id obcaecati facilis deserunt labore ullam dolores doloremque, animi velit eius illo incidunt asperiores! Est enim perferendis omnis!</p>
  </div>
</template>

<script setup>
const { id } = useRoute().params
</script>

<style   scoped>

</style>