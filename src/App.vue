<script setup>
import HeroSection from './components/HeroSection.vue'
import ScheduleList from './components/ScheduleList.vue'
import SignUpForm from './components/SignUpForm.vue'
</script>

<template>
  <HeroSection
    title="Bioengineering Week"
    tagline="Talks, workshops and good company."
    start-date="2026-11-16"
  />
  <ScheduleList />
  <SignUpForm />
  <footer>Made with Vue by the team</footer>
</template>

<style scoped>
footer {
  text-align: center;
  padding: 30px;
  color: #888;
}
</style>
