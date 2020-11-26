<template>
  <span>Current count is: {{ $store.state.count }}</span>
  <button v-on:click="$store.commit('changeCount', -1)">-</button>
  <button v-on:click="$store.commit('changeCount', 1)">+</button>
</template>

<script>
  export default {};
</script>