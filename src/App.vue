<!-- Vite uses script with setup, which is a new proposal. 
  For this demo, I am turning it off till I specifically take it. -->
<script lang="ts">
export default {
  data() {
    return {
      markup: '<p>Hello, there!</p>',
    };
  },
};
</script>

<template>
  <div class="p-5">
    <h2>Vue 3 Learning</h2>
    <hr />
    <!-- Vue automatically sanitizes the markup -->
    <div>This won't work: {{ markup }}</div>

    <!-- 
      v-html is a directive. 
      Use this carefully. 
      Sanitize user input. 
      Vue doesn't allow duplicate directives.
    -->
    <div v-html="markup"></div>
  </div>
</template>

<style scoped></style>
