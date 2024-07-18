<script setup>
import Navbar from './components/Navbar.vue';
import HeroSection from './components/HeroSection.vue';
import ClientSection from './components/ClientSection.vue';
import CommunitySection from './components/CommunitySection.vue';
import UnlockSection from './components/UnlockSection.vue';
import AchievementSection from './components/AchievementSection.vue';
import CalenderSection from './components/CalenderSection.vue';
import CustomerSection from './components/CustomerSection.vue';
import CommunityUpdateSection from './components/CommunityUpdateSection.vue';
import FooterSection from './components/Footer.vue';

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
    <CalenderSection />
    <CustomerSection />
    <CommunityUpdateSection />
  </main>

  <footer>
    <FooterSection />
  </footer>
</template>

<style scoped>
  header{
    background: #f5f7fa;
  }
</style>
