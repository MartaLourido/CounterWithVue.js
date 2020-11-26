<template>
  <span>Current count is: {{ count }}</span>
  <button v-on:click="$emit('update:count', count - 1)">-</button>
  <button v-on:click="$emit('update:count', count + 1)">+</button>
</template>

<script>
  export default {
    props: {
      count: Number
    }
  };
</script>