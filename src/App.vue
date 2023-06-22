<!-- Vite uses script with setup, which is a new proposal. 
  For this demo, I am turning it off till I specifically take it. -->
<script lang="ts">
export default {
  data() {
    return {
      isSelected: true,
    };
  },
};
</script>

<template>
  <div class="p-5">
    <h2>Vue 3 Learning</h2>
    <hr />
    <div class="form-check">
      <input class="form-check-input" type="checkbox" v-model="isSelected" />
    </div>
    <p v-show="isSelected">Checkbox is checked</p>

    <!-- v-show sets the display property to none if the predicate is false
    no v-else-if or v-else is allowed
    with large set of elements conditional rendering, where predicate 
    conditions are ephemeral, this can be an optimizing technique -->
  </div>
</template>

<style scoped></style>
