<template>
  <div>
    <h2>About Me</h2>
    <div class="grid grid-flow-row">
      <div>
        <h3 class="my-2">Past</h3>
        <div class="grid grid-flow-col">
          <aboutCard
            class="pl-4"
            v-for="(about, index) in pastAboutList"
            :key="index"
            :aboutText="about.aboutText"
          />
        </div>
      </div>
      <div>
        <h3 class="my-2">Present</h3>
        <div class="grid grid-flow-col">
          <aboutCard
            class="pl-4"
            v-for="(about, index) in presentAboutList"
            :key="index"
            :aboutText="about.aboutText"
          />
        </div>
      </div>
      <div>
        <h3 class="my-2">Future</h3>
        <div class="grid grid-flow-col">
          <aboutCard
            class="pl-4"
            v-for="(about, index) in futureAboutList"
            :key="index"
            :aboutText="about.aboutText"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const pastAboutList = [
  {
    aboutText: "I've been Geologist bla bla bla",
  },
];
const presentAboutList = [
  {
    aboutText:
      "I've been more than one year learning front-end, first throug a bootcamp and later doing my own projects",
  },
];
const futureAboutList = [
  {
    aboutText:
      "I'm gonna change careers to developing, because that is what moves me!",
  },
];
</script>

<style scoped></style>
