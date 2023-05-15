<template>
  <div>
    <h1>Usuario</h1>
  </div>
</template>
<script>
export default {
  mounted () {
    window.location.href = `https://api.arnoproducciones.com/usuario/${this.$route.params.dni}`
  }
}
</script>
