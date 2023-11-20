<template>
  <div>
    <h2>Skills</h2>
    <div class="grid grid-flow-col">
      <skillCard
        v-for="(skill, index) in skillList"
        :key="index"
        :skillTitle="skill.skillTitle"
        :skillText="skill.skillText"
      />
    </div>
  </div>
</template>

<script setup>
const skillList = [
  { skillTitle: "Javascript", skillText: "Javascript text" },
  { skillTitle: "Vue", skillText: "Vue text" },
  { skillTitle: "Nuxt", skillText: "Nuxt text" },
  { skillTitle: "CSS", skillText: "CSS text" },
];
</script>

<style scoped></style>
