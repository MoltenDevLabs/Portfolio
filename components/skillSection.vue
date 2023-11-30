<template>
  <div>
    <h2>Skills</h2>
    <div class="grid grid-flow-col grid-cols-3">
      <div class="flex flex-col items-center">
        <h3 class="my-2 underline">Main skills</h3>
        <div class="grid grid-flow-col">
          <skillCard
            class="px-2"
            v-for="(skill, index) in mainSkillList"
            :key="index"
            :skillTitle="skill.skillTitle"
          />
        </div>
      </div>
      <div class="flex flex-col items-center">
        <h3 class="my-2 underline">Aditional skills</h3>
        <div class="grid grid-flow-col">
          <skillCard
            class="px-2"
            v-for="(skill, index) in aditionalSkillList"
            :key="index"
            :skillTitle="skill.skillTitle"
          />
        </div>
      </div>
      <div class="flex flex-col items-center">
        <h3 class="my-2 underline">Soft skills</h3>
        <div class="grid grid-flow-col">
          <skillCard
            class="px-2"
            v-for="(skill, index) in softSkillList"
            :key="index"
            :skillTitle="skill.skillTitle"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const mainSkillList = [
  { skillTitle: "Javascript" },
  { skillTitle: "Vue & Nuxt" },
  { skillTitle: "CSS & Tailwind" },
];
const aditionalSkillList = [
  { skillTitle: "Git & Github" },
  { skillTitle: "Supabase" },
  { skillTitle: "Netlify" },
  { skillTitle: "AI" },
];
const softSkillList = [
  { skillTitle: "Creative thinking" },
  { skillTitle: "Problem solving" },
  { skillTitle: "Communication" },
  { skillTitle: "Open minded" },
];
</script>

<style scoped></style>
