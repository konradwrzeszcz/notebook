<template>
  <div id="app">
    <NoteViewer youtube-video-id="INEkjsEiQUg" />
    <NoteBrowser />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import VueYoutube from 'vue-youtube'
import NoteViewer from '@/views/NoteViewer.vue'
import NoteBrowser from '@/views/NoteBrowser.vue'

Vue.use(VueYoutube)

export default Vue.extend({
  name: 'App',
  components: {
    NoteViewer,
    NoteBrowser
  }
})
</script>
