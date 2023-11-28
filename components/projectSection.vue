<template>
  <div>
    <h2>Featured Projects</h2>
    <div class="grid grid-cols-3 gap-8">
      <projectCard
        v-for="(project, index) in projectList"
        :key="index"
        :projectImage="project.projectImage"
        :projectTitle="project.projectTitle"
        :projectType="project.projectType"
        :projectTag="project.projectTag"
        :projectText="project.projectText"
        :projectLink="project.projectLink"
      />
    </div>
  </div>
</template>

<script setup>
const projectList = [
  {
    projectImage:
      "https://lophahzsxonguopnjuyr.supabase.co/storage/v1/object/public/profile-pictures/defaultPfp.png",
    projectTitle: "Selecta Cakes",
    projectType: "e-commerce",
    projectTag: ["Responsive", "Design"],
    projectText: "Text here. a lot of text blah blah",
    projectLink: "",
  },
  {
    projectImage:
      "https://lophahzsxonguopnjuyr.supabase.co/storage/v1/object/public/profile-pictures/defaultPfp.png",
    projectTitle: "Coral Mussolidaria",
    projectType: "Community website",
    projectTag: ["Mobile", "Web app"],
    projectText: "Text here. a lot of text blah blah",
    projectLink: "",
  },
  {
    projectImage:
      "https://lophahzsxonguopnjuyr.supabase.co/storage/v1/object/public/profile-pictures/defaultPfp.png",
    projectTitle: "Playground",
    projectType: "playground",
    projectTag: ["Styles"],
    projectText: "Text here. a lot of text blah blah",
    projectLink: "",
  },
];
</script>

<style scoped></style>
