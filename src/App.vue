<template>
  <h1>{{ message }}</h1>
  <input type="text" placeholder="Your message..." v-model="message" />
  <br />
  <h1>The current count is {{ $store.state.count }}</h1>
  <!-- <counter v-bind:count="value" v-on:update:count="value = $event" /> -->
  <counter />
</template>

<script>
  import Counter from "./components/counter";
  export default {
    data() {
      return {
        message: "Hej världen!"
      };
    },
    components: {
      Counter
    }
  };
</script>

<style lang="scss">
  body {
    font-family: sans-serif;
  }
  h1 {
    text-decoration: underline;
  }
</style>
