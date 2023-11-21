<template>
  <div>
    <div
      class="relative hover:scale-105 transition-all ease-in-out duration-500 backdrop-blur-sm flex flex-col justify-center items-center align-middle w-full aspect-square p-4 border outline-offset-0 rounded-lg shadow shadow-slate-800/40 dark:shadow-slate-300/40"
    >
      <span class="absolute chip top-5 right-5">
        {{ projectType }}
      </span>
      <div class="mb-0">
        <img
          class="m-0 rounded-t-lg w-24 hover:scale-125 transition-all ease-in-out duration-500"
          :src="projectImage"
          alt="Project photo"
        />
      </div>
      <div class="mt-0 rounded-b-lg">
        <h4 class="mt-0 pt-4 px-4">{{ projectTitle }}</h4>
      </div>
      <div class="absolute bottom-5 flex justify-center items-center flex-wrap">
        <span v-for="(tag, index) in projectTag" :key="index" class="chip m-1">
          {{ tag }}
        </span>
      </div>
    </div>
  </div>
</template>

<script setup>
defineProps({
  projectImage: {
    type: String,
    required: true,
  },
  projectTitle: {
    type: String,
    required: true,
  },
  projectText: {
    type: String,
    required: true,
  },
  projectType: {
    type: String,
    required: true,
  },
  projectTag: {
    type: Array,
    required: true,
  },
});
</script>

<style scoped></style>
