<template>
  <youtube :video-id="youtubeVideoId" />
</template>

<script lang="ts">
import { Vue, Component, Prop } from 'vue-property-decorator'

@Component
export default class NoteViewer extends Vue {
  @Prop() youtubeVideoId!: string
}
</script>
