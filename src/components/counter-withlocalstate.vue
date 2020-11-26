<template>
  <span>Current count is: {{ count }}</span>
  <button v-on:click="count--">-</button>
  <button v-on:click="count++">+</button>
</template>

<script>
  export default {
    data() {
      return {
        count: 0
      };
    }
  };
</script>