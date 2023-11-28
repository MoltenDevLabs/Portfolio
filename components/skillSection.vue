<template>
  <div>
    <h2>Skills</h2>
    <div class="grid grid-flow-row">
      <div>
        <h3 class="mb-2">Main skills</h3>
        <div class="grid grid-flow-col">
          <skillCard
            class="pl-4"
            v-for="(skill, index) in mainSkillList"
            :key="index"
            :skillTitle="skill.skillTitle"
            :skillText="skill.skillText"
          />
        </div>
      </div>
      <div>
        <h3 class="mb-2">Aditional skills</h3>
        <div class="grid grid-flow-col">
          <skillCard
            class="pl-4"
            v-for="(skill, index) in aditionalSkillList"
            :key="index"
            :skillTitle="skill.skillTitle"
            :skillText="skill.skillText"
          />
        </div>
      </div>
      <div>
        <h3 class="mb-2">Soft skills</h3>
        <div class="grid grid-flow-col">
          <skillCard
            class="pl-4"
            v-for="(skill, index) in softSkillList"
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
  {
    skillTitle: "Javascript",
    skillText: "",
  },
  { skillTitle: "Vue & Nuxt", skillText: "" },
  { skillTitle: "CSS & Tailwind", skillText: "" },
];
const aditionalSkillList = [
  { skillTitle: "Git & Github", skillText: "" },
  { skillTitle: "Supabase", skillText: "" },
  { skillTitle: "Netlify", skillText: "" },
  { skillTitle: "AI", skillText: "" },
];
const softSkillList = [
  { skillTitle: "Creative thinking", skillText: "" },
  { skillTitle: "Problem solving", skillText: "" },
  { skillTitle: "Communication", skillText: "" },
  { skillTitle: "Open minded", skillText: "" },
];
</script>

<style scoped></style>
