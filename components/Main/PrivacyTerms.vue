<template>
  <div style="display:grid;place-items:center;" @click="dialog = true">
    <v-icon class="text-h1 d-block mx-auto">
      mdi-file-document-check-outline
    </v-icon>
    <span class="text-subtitle-1">Politica de Tratamiento de Datos</span>
    <v-dialog
      v-model="dialog"
      width="90%"
    >
      <v-card>
        <v-card-title class="text-h5 grey lighten-2">
          Conoce nuestra politica de tratamiento de tus datos
        </v-card-title>

        <v-card-text>
          <a href="https://arnoproducciones.com/doc/A SAS - POLITICA DE TRATAMIENTO DE DATOS.pdf">Descargar PDF</a>
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
