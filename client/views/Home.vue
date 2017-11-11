<template>
  <div class="page">
    <search-character-form></search-character-form>
    <characters-list></characters-list>
  </div>
</template>

<script>
import Counter from 'components/Counter'
import SearchCharacterForm from 'components/SearchCharacterForm'
import CharactersList from 'components/CharactersList'

export default {
  components: {
    Counter,
    SearchCharacterForm,
    CharactersList
  }
}
</script>
