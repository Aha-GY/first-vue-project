<template>
  <div>
    <detailSocialMediaPage />
    <MediaCard/>
  </div>
</template>

<script>
import detailSocialMediaPage from './components/detail-social-media-page.vue'
import MediaCard from './components/MediaCard.vue'

export default {
  components: {
    detailSocialMediaPage,
    MediaCard
  },
  
};
</script>
