<template>
  <div style="display:grid;place-items:center;" @click="dialog = true">
    <v-icon class="text-h1 d-block mx-auto">
      mdi-speedometer
    </v-icon>
    <span class="text-subtitle-1">Medidor de Velocidad</span>
    <v-dialog
      v-model="dialog"
      width="90%"
    >
      <v-card>
        <v-card-title class="text-h5 grey lighten-2">
          Medidor de velocidad de tu red
        </v-card-title>

        <v-card-text>
          Recuerda que la prueba solo sera precisa si realizas la misma desde un computador conectado por cable. Al hacerlo por WiFi tendras interferencias que no permitiran que la prueba sea precisa.
        </v-card-text>

        <v-card-text v-if="dialog">
          <iframe width="100%" height="650px" frameborder="0" src="https://arnoproducciones.speedtestcustom.com" />
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
