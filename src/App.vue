<!-- Vite uses script with setup, which is a new proposal. 
  For this demo, I am turning it off till I specifically take it. -->
<script lang="ts">
import persons from './data.json';
export default {
  data() {
    return {
      persons,
    };
  },
};
</script>

<template>
  <div class="p-5">
    <h2>Vue 3 Learning</h2>
    <hr />
    <div
      class="alert alert-primary"
      role="alert"
      v-for="(person, index) in persons"
      :key="person.id"
    >
      <p>Serial: {{ index }}</p>
      <p>First Name: {{ person.firstName }}</p>
      <p>Last Name: {{ person.lastName }}</p>
      <p>Email: {{ person.email }}</p>
    </div>

    <!-- index is optional
    by default index is used as key prop
    more about key prop: https://vuejs.org/api/built-in-special-attributes.html#key
     -->
  </div>
</template>

<style scoped></style>
