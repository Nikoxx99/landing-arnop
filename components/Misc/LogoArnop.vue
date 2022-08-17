<template>
  <div class="d-grid place-items-end" style="display:grid;place-items:end end;">
    <v-img src="logo-dark.png" :max-width="width" />
  </div>
</template>
<script>
export default {
  props: {
    width: {
      type: String,
      default: '30vw'
    }
  }
}
</script>
