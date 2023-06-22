<!-- Vite uses script with setup, which is a new proposal. 
  For this demo, I am turning it off till I specifically take it. -->
<script lang="ts">
export default {
  data() {
    return {
      message: 'Good day!',
      uniqueId: 'app-el-1',
      fullName: 'John Doe',
      isReadOnly: true,
    };
  },
};
</script>

<template>
  <div class="p-5">
    <h2>Vue 3 Learning</h2>
    <hr />
    <p v-bind:title="message" v-bind:id="uniqueId">{{ fullName }}</p>
    <!-- v-bind can be skipped, retaining only the colon -->
    <p :title="message" :id="uniqueId">{{ fullName }}</p>
    <input
      type="text"
      class="form-control"
      :value="message"
      :readonly="isReadOnly"
    />
  </div>
</template>

<style scoped></style>
