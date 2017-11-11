<template>
  <div class="counter-wrapper">
    <div class="counter">
      {{ data }}
    </div>
    <button @click="fetchCharacters('wolverine')">Fetch</button>
  </div>
</template>

<script>
import { mapState, mapActions } from 'vuex'

export default {
  computed: mapState([
    'data'
  ]),
  methods: mapActions([
    'fetchCharacters'
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
