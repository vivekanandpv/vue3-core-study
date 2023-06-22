<!-- Vite uses script with setup, which is a new proposal. 
  For this demo, I am turning it off till I specifically take it. -->
<script lang="ts">
export default {
  data() {
    return {
      isRegistered: true,
    };
  },
};
</script>

<template>
  <div class="p-5">
    <h2>Vue 3 Learning</h2>
    <hr />
    <!-- Only expressions are allowed. Statements, such as assignment, 
    branching, etc are not allowed in templates. -->
    <p>{{ isRegistered ? 'Registered' : 'Not Registered' }}</p>
  </div>
</template>

<style scoped></style>
