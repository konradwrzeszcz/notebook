<template>
  <YoutubeThumbnail :youtube-video-id="youtubeVideoId" />
</template>

<script lang="ts">
import { Vue, Component } from 'vue-property-decorator'
import YoutubeThumbnail from '@/components/YoutubeThumbnail.vue'

@Component({
  components: {
    YoutubeThumbnail
  }
})
export default class NoteBrowser extends Vue {
  youtubeVideoId = 'INEkjsEiQUg'
}
</script>
