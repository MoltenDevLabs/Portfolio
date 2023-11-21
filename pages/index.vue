<template>
  <div>
    <!-- HERO SECTION -->
    <heroSection class="relative mb-40 md:mb-44 mt-20 md:mt-12" />
    <!-- SECTION ONE SECTION -->
    <skillSection class="fade-in-effect mb-24" />
    <!-- SECTION TWO SECTION -->
    <projectSection class="fade-in-effect mb-24" />
    <!-- SECTION THREE SECTION-->
    <sectionThreeSection class="fade-in-effect mb-24" />
    <!-- SECTION FOUR SECTION -->
    <sectionFourSection class="fade-in-effect" />
  </div>
</template>

<script setup>
useFadeInEffect();

onMounted(() => {
  window.scrollTo({
    top: 0,
    behavior: "smooth",
  });
});
</script>

<style></style>
