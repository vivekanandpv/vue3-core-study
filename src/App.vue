<!-- Vite uses script with setup, which is a new proposal. 
  For this demo, I am turning it off till I specifically take it. -->
<script lang="ts">
export default {
  data() {
    return {
      person: {
        id: 4,
        firstName: 'Michele',
        lastName: 'Thorneywork',
        email: 'mthorneywork3@fastcompany.com',
        ipAddress: '61.47.243.3',
      },
    };
  },
};
</script>

<template>
  <div class="p-5">
    <h2>Vue 3 Learning</h2>
    <hr />
    <div class="alert alert-primary" role="alert">
      <p v-for="(value, key, index) in person">
        {{ index }} --> {{ key }}: {{ value }}
      </p>
    </div>

    <!-- In object iteration, key and index are optional -->
  </div>
</template>

<style scoped></style>
