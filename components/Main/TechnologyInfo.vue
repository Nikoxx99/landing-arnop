<template>
  <div style="display:grid;place-items:center;" @click="dialog = true">
    <v-icon class="text-h1 d-block mx-auto">
      mdi-router-wireless
    </v-icon>
    <span class="text-subtitle-1">Tecnologías</span>
    <v-dialog
      v-model="dialog"
      width="90%"
    >
      <v-card>
        <v-card-title class="text-h5 grey lighten-2">
          La tecnologia que usamos para brindar tu servicio
        </v-card-title>

        <v-card-text>
          <a href="#">Descargar PDF</a>
        </v-card-text>

        <v-divider />

        <v-card-actions>
          <v-btn
            color="primary"
            @click="dialog = false"
          >
            Finalizar
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-dialog>
  </div>
</template>
<script>
export default {
  data () {
    return {
      dialog: false
    }
  }
}
</script>
