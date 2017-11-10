<template>
  <div class="counter-wrapper">
    <div class="counter">
      {{ count }}
    </div>
    <button @click="this.increment">Increment</button>
    <button @click="this.decrement">Decrement</button>
    <button @click="this.incrementAsync">Increment Async</button>
  </div>
</template>

<script>
import { mapState, mapActions } from 'vuex'

export default {
  computed: mapState([
    'count'
  ]),
  methods: mapActions([
    'incrementAsync',
    'increment',
    'decrement'
  ])
}
</script>

<style>
.counter {
  margin: 100px auto;
  border-radius: 3px;
  width: 200px;
  height: 200px;
  text-align: center;
  line-height: 200px;
  font-size: 5rem;
  background-color: #f0f0f0;
  user-select: none;
}
</style>
