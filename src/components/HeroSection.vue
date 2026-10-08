<script setup>
import { computed } from 'vue'

// Values passed in from App.vue
const props = defineProps({
  title: String,
  tagline: String,
  startDate: String,
})

const daysLeft = computed(() => {
  const ms = new Date(props.startDate) - new Date()
  return Math.max(0, Math.ceil(ms / (1000 * 60 * 60 * 24)))
})
</script>

<template>
  <header class="hero">
    <h1>{{ title }}</h1>
    <p>{{ tagline }}</p>
    <p class="countdown">{{ daysLeft }} days to go!</p>
  </header>
</template>

<style scoped>
.hero {
  background: var(--main);
  color: white;
  text-align: center;
  padding: 60px 20px;
}

h1 {
  margin: 0 0 10px;
  font-size: 2.5rem;
}

.countdown {
  font-weight: bold;
}
</style>
