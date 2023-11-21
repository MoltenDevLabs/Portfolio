<template>
  <div>
    <h2>Skills</h2>
    <div class="grid grid-flow-row">
      <div>
        <h3>Main skills</h3>
        <div class="grid grid-flow-col">
          <skillCard
            v-for="(skill, index) in mainSkillList"
            :key="index"
            :skillTitle="skill.skillTitle"
            :skillText="skill.skillText"
          />
        </div>
      </div>
      <div>
        <h3>Aditional skills</h3>
        <div class="grid grid-flow-col">
          <skillCard
            v-for="(skill, index) in aditionalSkillList"
            :key="index"
            :skillTitle="skill.skillTitle"
            :skillText="skill.skillText"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const mainSkillList = [
  { skillTitle: "Javascript", skillText: "Javascript text" },
  { skillTitle: "Vue & Nuxt", skillText: "Vue text" },
  { skillTitle: "CSS & Tailwind", skillText: "CSS text" },
];
const aditionalSkillList = [
  { skillTitle: "Git & Github", skillText: "Git & Github text" },
  { skillTitle: "Supabase", skillText: "Supabase text" },
  { skillTitle: "Netlify", skillText: "Netlify text" },
  { skillTitle: "AI", skillText: "Text, code, images, etc" },
];
</script>

<style scoped></style>
