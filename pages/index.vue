<template>
  <div>
    <!-- NAVBAR SECTION -->
    <navbarSection id="header" />
    <!-- HERO SECTION -->
    <heroSection id="heroSection" class="relative mb-28 mt-8 pt-0.5" />
    <!-- SKILL SECTION -->
    <skillSection id="skillSection" class="fade-in-effect mb-28 mt-8 pt-0.5" />
    <!-- PROJECT SECTION -->
    <projectSection
      id="projectSection"
      class="fade-in-effect mb-28 mt-8 pt-0.5"
    />
    <!-- ABOUT SECTION-->
    <aboutSection id="aboutSection" class="fade-in-effect mb-28 mt-8 pt-0.5" />
    <!-- CONTACT SECTION -->
    <contactSection
      id="contactSection"
      class="fade-in-effect mb-28 mt-8 pt-0.5"
    />
    <!-- FOOTER SECTION -->
    <footerSection />
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
