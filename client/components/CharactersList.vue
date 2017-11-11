<template>
  <div v-If="!!characters.length" class="ui characters-list cards">
    <div v-for="character in characters" :key="character.name" class="ui card fadeIn-animation">
      <div class="image">
          <img :src="character.image" />
      </div>
      <div class="content">
        <div class="header">{{character.name}}</div>
        <div class="description">
          {{character.description}}
        </div>
      </div>
      <div class="extra content">
        <span class="right floated">
          <a target="_blank" :href="character.url">
            <button class="ui icon purple tiny button">
                More Info
            </button>
          </a>
        </span>
      </div>
    </div>
  </div>
</template>

<script>
import { mapGetters } from 'vuex'

export default {
  computed: mapGetters([
    'characters'
  ])
}
</script>
