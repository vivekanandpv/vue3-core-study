<!-- Vite uses script with setup, which is a new proposal. 
  For this demo, I am turning it off till I specifically take it. -->
<script lang="ts">
export default {
  data() {
    //  The object returned by data function becomes the part of
    //  Vue reactivity system. It will be available as this.counter
    //  once the component instance springs up
    return {
      counter: 0,
    };
  },
  methods: {
    increment() {
      //  changes the counter in the reactivity system
      ++this.counter;
    },
    decrement() {
      //  changes the counter in the reactivity system
      --this.counter;
    },
  },
};
</script>

<template>
  <div class="p-5">
    <h2>Vue 3 Learning</h2>
    <hr />

    <!-- This binding gets evaluated when the 
    counter changes in the reactivity system -->
    <h3 class="mb-3">Counter: {{ counter }}</h3>

    <button class="btn btn-primary me-4" @click="increment">Increment</button>
    <button class="btn btn-danger" @click="decrement">Decrement</button>
  </div>
</template>

<style scoped></style>
