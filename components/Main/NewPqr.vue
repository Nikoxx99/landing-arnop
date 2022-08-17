<template>
  <div style="display:grid;place-items:center;" @click="dialog = true">
    <v-icon class="text-h1 d-block mx-auto">
      mdi-email-newsletter
    </v-icon>
    <span class="text-subtitle-1">Radicar PQR</span>
    <v-dialog
      v-model="dialog"
      width="90%"
    >
      <v-card>
        <v-card-title class="text-h5 grey lighten-2">
          En este apartado puedes generar tu PQR
        </v-card-title>

        <v-card-text>
          <a href="mailto:arnaldopalomino1234@hotmail.com">Redactar PQR</a>
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
