<!-- Vite uses script with setup, which is a new proposal. 
  For this demo, I am turning it off till I specifically take it. -->
<script lang="ts">
export default {
  data() {
    return {
      score: 5,
    };
  },
};
</script>

<template>
  <div class="p-5">
    <h2>Vue 3 Learning</h2>
    <hr />
    <p class="fw-bold" v-if="score >= 4">Good</p>
    <p class="fw-bold" v-else-if="score >= 2">Average</p>
    <p class="fw-bold" v-else>Poor</p>
    <!-- First v-else-if must follow v-if
    multiple v-else-if are allowed
    no intervening elements are allowed
    v-else-if alone is not allowed
    v-else-if is optional
    v-else-if takes the predicate value
    v-else is optional -->

    <select
      class="form-select mt-4"
      aria-label="Default select example"
      v-model="score"
    >
      <option value="1">One</option>
      <option value="2">Two</option>
      <option value="3">Three</option>
      <option value="4">Four</option>
      <option value="5">Five</option>
    </select>

    <!-- v-else is optional
    there should not be any intervening elements between v-if and v-else
    if there are multiple v-if, v-else is applicable to the one that is adjacent
    multiple v-else are not allowed
    v-else doesn't take any value -->
  </div>
</template>

<style scoped></style>
