<template>
  <div class="page">
    <search-character-form>
    </search-character-form>
    <counter></counter>
    <p>
      To get started, edit files in <code>./client</code> and save.
    </p>
  </div>
</template>

<script>
import Counter from 'components/Counter'
import SearchCharacterForm from 'components/SearchCharacterForm'

export default {
  components: {
    Counter,
    SearchCharacterForm
  }
}
</script>
