<template>
  <div>
    <h1>Counter!!!</h1>
    <p>{{count}}</p>
    <button @click="increment">+</button>
    <button @click="decrement">-</button>
  </div>
</template>

<script>
import { mapState, mapActions } from 'vuex';
export default {
  name: 'Counter',
  computed: mapState(['count']),
  methods: {
    ...mapActions(['increment', 'decrement'])
  }
};
</script>

<style scoped>
</style>