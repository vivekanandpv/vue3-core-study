<!-- Vite uses script with setup, which is a new proposal. 
  For this demo, I am turning it off till I specifically take it. -->
<script lang="ts">
export default {
  data() {
    return {
      message: 'Greetings!',
      year: 2023,
      isRegistered: true,
    };
  },
  methods: {
    getRandomNumber() {
      return Math.random();
    },
  },
};
</script>

<template>
  <div class="p-5">
    <h2>Vue 3 Learning</h2>
    <hr />
    <p>Message: {{ message }}</p>
    <p>Year: {{ year }}</p>
    <p>Random Number: {{ getRandomNumber() }}</p>
  </div>
</template>

<style scoped></style>
