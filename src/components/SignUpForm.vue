<script setup>
import { ref } from 'vue'

const name = ref('')
const email = ref('')
const message = ref('')
const attendees = ref([])

function signUp() {
  attendees.value.push({ name: name.value, email: email.value })
  message.value = `Thanks, ${name.value}! See you there.`
  name.value = ''
  email.value = ''
}
</script>

<template>
  <section>
    <h2>Sign up</h2>

    <form @submit.prevent="signUp">
      <input v-model="name" placeholder="Your name" required />
      <input v-model="email" type="email" placeholder="Your email" required />
      <button type="submit">Join us!</button>
    </form>

    <p v-if="message" class="message">{{ message }}</p>
    <p>{{ attendees.length }} people signed up so far.</p>
  </section>
</template>

<style scoped>
form {
  display: flex;
  flex-direction: column;
  gap: 10px;
}

input {
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 6px;
  font-size: 1rem;
}

.message {
  color: var(--main);
  font-weight: bold;
}
</style>
