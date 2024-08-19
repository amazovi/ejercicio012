<template>
    <div>
      <button :style="{ backgroundColor: buttonColor }" @click="changeColor">Click me</button>
    </div>
  </template>
  
  <script setup>
  import { ref } from 'vue';
  
  const buttonColor = ref('red');
  
  const changeColor = () => {
    buttonColor.value = buttonColor.value === 'blue' ? 'green' : 'blue';
  };
  </script>
  
  <style scoped>
  button {
    padding: 0.5rem 1rem;
    border: none;
    color: white;
    cursor: pointer;
    margin-top: 1rem;
  }
  </style>