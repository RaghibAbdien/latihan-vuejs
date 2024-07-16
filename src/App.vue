<script setup>
import Navbar from './components/Navbar.vue';
import HeroSection from './components/HeroSection.vue';
import ClientSection from './components/ClientSection.vue';
import CommunitySection from './components/CommunitySection.vue';
import UnlockSection from './components/UnlockSection.vue';
import AchievementSection from './components/AchievementSection.vue';

</script>

<template>
  <header>
    <Navbar />
    <HeroSection />
  </header>

  <main>
    <ClientSection />
    <CommunitySection />
    <UnlockSection />
    <AchievementSection />
  </main>
</template>

<style scoped>
  header{
    background: #f5f7fa;
  }
</style>
