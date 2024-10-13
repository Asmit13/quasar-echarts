<template>
  <div>
    <h2>Random Number Generator</h2>
    <p>Click the button to generate a random number between 1 and 100:</p>
    <button @click="generateRandomNumber">Generate Random Number</button>
    <p>Random Number: {{ randomNumber }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      randomNumber: 0,
    };
  },
  methods: {
    generateRandomNumber() {
      this.randomNumber = Math.floor(Math.random() * 100) + 1;
    },
  },
};
</script>

<style scoped>
/* Add your custom styles here */
</style>
