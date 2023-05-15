<template>
  <video id="video" style="width:100% !important;,height:auto !important;" controls muted />
</template>

<script>
export default {
  name: 'LivePage',
  layout: 'video'
}
</script>
<style scoped>
.frosted {
  background-color: rgba(255, 255, 255, 0.5)!important;
  backdrop-filter: blur(20px)!important;
}
audio::-webkit-media-controls-timeline,
video::-webkit-media-controls-timeline,
video::-webkit-media-controls-current-time-display,
video::-webkit-media-controls-time-remaining-display {
    display: none;
}
</style>
