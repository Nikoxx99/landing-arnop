<template>
  <div style="display:grid;place-items:center;" @click="dialog = true">
    <v-icon class="text-h1 d-block mx-auto">
      mdi-text-box-plus-outline
    </v-icon>
    <span class="text-subtitle-1">Contratos</span>
    <v-dialog
      v-model="dialog"
      width="90%"
    >
      <v-card>
        <v-card-title class="text-h5 grey lighten-2">
          Nuestros contratos de servicio
        </v-card-title>

        <v-card-text>
          <a href="https://arnoproducciones.com/doc/A SAS - CONTRATO INTERNET.pdf">Contrato de Internet (Descargar PDF)</a> <br>
          <a href="https://arnoproducciones.com/doc/A SAS - TERMINOS FACTURA Y-O ESTADO DE CUENTA DIGITAL.pdf">Terminos y condiciones Factura y/o estado de cuenta digital (Descargar PDF)</a>
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
