<template>
  <div>
    <h4>{{ skillTitle }}</h4>
    <p>{{ skillText }}</p>
  </div>
</template>

<script setup>
defineProps({
  skillTitle: String,
  skillText: String,
});
</script>

<style scoped></style>
