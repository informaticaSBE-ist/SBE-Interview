<script setup>
import { ref, computed } from 'vue'
import { activities } from '../data/activities.js'

const selectedDay = ref('All')

// "All" + every day that appears in the schedule
const days = computed(() => ['All', ...new Set(activities.map((a) => a.day))])

// Only the activities for the selected day
const filteredActivities = computed(() => {
  if (selectedDay.value === 'All') return activities
  return activities.filter((a) => a.day === selectedDay.value)
})
</script>

<template>
  <section>
    <h2>Schedule</h2>

    <div class="filters">
      <button
        v-for="day in days"
        :key="day"
        :class="{ active: day === selectedDay }"
        @click="selectedDay = day"
      >
        {{ day }}
      </button>
    </div>

    <div class="card" v-for="activity in filteredActivities" :key="activity.title">
      <span class="time">{{ activity.time }}</span>
      <h3>{{ activity.title }}</h3>
      <p>{{ activity.speaker }}</p>
    </div>
  </section>
</template>

<style scoped>
.filters {
  margin-bottom: 15px;
}

.card {
  background: white;
  border-radius: 10px;
  padding: 15px;
  margin-bottom: 10px;
  box-shadow: 0 2px 6px rgba(0, 0, 0, 0.1);
}

.card h3 {
  margin: 5px 0;
}

.card p {
  margin: 0;
  color: #666;
}

.time {
  color: var(--main);
  font-weight: bold;
}
</style>
