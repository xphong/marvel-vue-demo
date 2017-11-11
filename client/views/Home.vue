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

<<style>
@import url(https://fonts.googleapis.com/css?family=Lato);

body {
  background-color: #f1f2f0;
  color: #35342f;
  display: flex;
  justify-content: center;
  font-family: 'Lato', sans-serif;
}

.page {
  margin: 80px auto;
}
</style>
