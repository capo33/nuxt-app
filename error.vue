<template>
  <div class="grid h-screen px-4 bg-white place-content-center">
    <div class="text-center">
      <h1 class="font-black text-gray-200 text-9xl">{{ error.statusCode }}</h1>

      <p class="text-2xl font-bold tracking-tight text-gray-900 sm:text-4xl">
        Uh-oh!
      </p>
      <p class="mt-4 text-gray-500">{{ error.message }}</p>
      <button class="btn my-7" @click="handleClearError">Go Home...</button>
    </div>
  </div>
</template>

<script setup>
defineProps(["error"]);

const handleClearError = () => clearError({ redirect: "/" , });
</script>
