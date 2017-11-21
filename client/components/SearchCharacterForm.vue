<template>
  <div class="search-character__form">
    <form @submit.prevent="handleSearch()">

      <div class="ui action input">
        <input v-model="name"
          placeholder="Character Name"
          type="text"
          required />

          <button class="ui icon pink button">
            <i class="search icon"></i>
          </button>
      </div>
    </form>
  </div>
</template>

<script>
export default {
  data: function () {
    return {
      name: ''
    }
  },
  methods: {
    handleSearch () {
      this.$store.dispatch('FETCH_CHARACTERS', this.name)
    }
  }
}
</script>
