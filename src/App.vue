<!-- Vite uses script with setup, which is a new proposal. 
  For this demo, I am turning it off till I specifically take it. -->
<script lang="ts">
export default {
  methods: {
    handleClick(e: MouseEvent) {
      console.log('Clicked', e);
    },
  },
};
</script>

<template>
  <div class="p-5">
    <h2>Vue 3 Learning</h2>
    <hr />
    <!-- @click is a shorthand for v-on:click
    assign the handler reference, do not call the handler
    accepting the event args in the handler is optional
    use type-safe programming in Vue 3 -->
    <button class="btn btn-primary" @click="handleClick">Click Here</button>
  </div>
</template>

<style scoped></style>
