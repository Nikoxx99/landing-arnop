<template>
  <div style="display:grid;place-items:center;" @click="dialog = true">
    <v-icon class="text-h1 d-block mx-auto">
      mdi-laptop
    </v-icon>
    <span class="text-subtitle-1">Medidas de gestión de tráfico</span>
    <v-dialog
      v-model="dialog"
      width="90%"
    >
      <v-card>
        <v-card-title class="text-h5 grey lighten-2">
          Estas son las medidas que tomamos para proteger tu tráfico en linea
        </v-card-title>

        <v-card-text>
          Las siguientes prácticas de gestión de tráfico están enmarcadas en la resolución 3502 de 2.011 de la CRC que establece las condiciones regulatorias relacionadas con la neutralidad de la red.

          Los servicios internet Masivo y Corporativo prestados por ARNO PRODUCCIONES S.A.S. son ilimitados. Esto quiere decir, que sin importar cuánto tráfico sea descargado o subido, se mantiene la misma velocidad y condiciones del servicio.

          Para los servicios se usa una navegacion simetrica con reuso de 1:1 mientras el ancho de banda lo permita. En horas pico se puede llegar a realizar hasta un reuso de 1:4. Esta ultima medida solo se aplicara luego de las 5pm y si el ancho de banda total disponible por la empresa supera el 95% de uso.

          Para realizar las mediciones de velocidad por favor dirigirse al item de Medidor de Velocidad presente en el indice de esta página web.
        </v-card-text>

        <v-divider />

        <v-card-actions>
          <v-btn
            color="primary"
            @click="dialog = false"
          >
            Cerrar
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
