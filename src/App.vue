<!-- Vite uses script with setup, which is a new proposal. 
  For this demo, I am turning it off till I specifically take it. -->
<script lang="ts">
export default {
  data() {
    return {
      message: 'Good day!',
    };
  },
};
</script>

<template>
  <div class="p-5">
    <h2>Vue 3 Learning</h2>
    <hr />

    <p>Message: {{ message }}</p>

    <!-- v-model can only be applied to input, select, and textarea elements -->
    <input type="text" class="form-control" v-model="message" />
  </div>
</template>

<style scoped></style>
