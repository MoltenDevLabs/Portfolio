<template>
  <div>
    <p class="mb-6 mt-2">{{ aboutText }}</p>
  </div>
</template>

<script setup>
defineProps({
  aboutText: String,
});
</script>

<style scoped></style>
