<template>
  <div class="page">
    <search-character-form></search-character-form>
    <characters-list></characters-list>
  </div>
</template>

<script>
import SearchCharacterForm from 'components/SearchCharacterForm'
import CharactersList from 'components/CharactersList'

export default {
  components: {
    SearchCharacterForm,
    CharactersList
  }
}
</script>
