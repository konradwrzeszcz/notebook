<template>
  <img :src="youtubeThumbnailLink" />
</template>

<script lang="ts">
import { Vue, Component, Prop } from 'vue-property-decorator'

@Component
export default class YoutubeThumbnail extends Vue {
  @Prop() youtubeVideoId!: string

  get youtubeThumbnailLink(): string {
    return `https://img.youtube.com/vi/${this.youtubeVideoId}/mqdefault.jpg`
  }
}
</script>
