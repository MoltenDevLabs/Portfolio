<template>
  <div>
    <!-- HERO SECTION -->
    <heroSection class="relative mb-24" />
    <!-- SKILL SECTION -->
    <skillSection class="fade-in-effect mb-24" />
    <!-- PROJECT SECTION -->
    <projectSection class="fade-in-effect mb-24" />
    <!-- ABOUT SECTION-->
    <aboutSection class="fade-in-effect mb-24" />
    <!-- CONTACT SECTION -->
    <contactSection class="fade-in-effect" />
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
