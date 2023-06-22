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
    <p v-if="isSelected">Checkbox is checked</p>
    <p v-else>Checkbox is unchecked</p>

    <!-- v-else is optional
    there should not be any intervening elements between v-if and v-else
    if there are multiple v-if, v-else is applicable to the one that is adjacent
    multiple v-else are not allowed
    v-else doesn't take any value -->
  </div>
</template>

<style scoped></style>
