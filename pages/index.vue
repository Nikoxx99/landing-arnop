<template>
  <v-container fluid>
    <v-row>
      <MainHeroLanding />
    </v-row>
    <v-row style="margin-top:-100px;" class="mb-5">
      <v-col cols="12" md="6" lg="6" class="d-flex justify-center justify-md-end justify-lg-end">
        <v-card width="500" class="pt-3 frosted">
          <v-img
            width="200"
            class="mx-auto"
            src="svg/internet.svg"
          />
          <v-card-title class="justify-center mt-5 text-h5 font-weight-bold blue--text darken-4">
            Internet Ilimitado por Fibra Óptica
          </v-card-title>
          <v-card-text class="align-center text-center white--text justify-center blue lighten-1 pt-4">
            <div class="align-center text-h5 my-2">
              Con velocidades desde 8 Megas
            </div>

            <div>Para el hogar y toda tu familia. Conectividad cuando lo necesitas y para lo que lo necesitas</div>
          </v-card-text>
        </v-card>
      </v-col>
      <v-col cols="12" md="6" lg="6" class="d-flex justify-center justify-md-start justify-lg-start">
        <v-card width="500" class="pt-3 frosted">
          <v-img
            width="200"
            class="mx-auto"
            src="svg/television.svg"
          />
          <v-card-title class="justify-center mt-5 text-h5 font-weight-bold blue--text darken-4">
            Televisión por Cable
          </v-card-title>
          <v-card-text class="align-center text-center white--text justify-center blue lighten-1 pt-4" style="position:absolute;bottom:0;">
            <div class="align-center text-h5 my-2">
              90 Canales SD y 24 Canales HD
            </div>

            <div>El mejor entrenemiento, peliculas de estreno y lo ultimo en deporte para que disfrutes en familia</div>
          </v-card-text>
        </v-card>
      </v-col>
    </v-row>
    <v-row justify="center" align="center" class="mb-5 mt-0">
      <v-col class="justify-center d-flex" cols="12">
        <v-card class="justify-center frosted" width="1024">
          <video id="video" style="width:100% !important;,height:auto !important;" controls muted />
          <v-card-actions>
            <span class="text-subtitle-1">Canal regional +NorteTv en Vivo 🔴</span>
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>
    <v-row justify="center" align="center" class="mb-5 mt-0">
      <v-col class="justify-center d-flex pt-0" cols="12">
        <v-card class="justify-center frosted" width="1024">
          <v-card-title class="justify-center">
            Información importante para usuarios
          </v-card-title>
          <v-card-text class="text-center">
            <p>Aquí podra encontrar informacion que como usuarios, debe conocer acerca del servicio</p>
          </v-card-text>
          <v-card-text>
            <v-row class="mb-10 text-center">
              <v-col>
                <MainSpeedMeter />
              </v-col>
              <v-col>
                <MainPrivacyTerms />
              </v-col>
              <v-col>
                <MainTechnologyInfo />
              </v-col>
            </v-row>
            <v-row class="mb-10 text-center">
              <v-col>
                <MainFiledMaintenance />
              </v-col>
              <v-col>
                <MainContractInfo />
              </v-col>
              <v-col>
                <MainUserRights />
              </v-col>
            </v-row>
            <v-row class="mb-10 text-center">
              <v-col>
                <MainNewPqr />
              </v-col>
              <v-col>
                <MainTrafficActions />
              </v-col>
              <v-col>
                <MainGoodPractices />
              </v-col>
            </v-row>
          </v-card-text>
        </v-card>
      </v-col>
    </v-row>
    <v-row class="mb-5 mt-0">
      <v-col class="justify-center d-flex">
        <v-card class="frosted" width="1024">
          <v-card-text>
            <MainMapLocation />
          </v-card-text>
        </v-card>
      </v-col>
    </v-row>
    <v-row class="justify-center mb-5">
      <v-col class="justify-center d-flex">
        <MainFooterView />
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: 'IndexPage'
}
</script>
<style scoped>
.frosted {
  background: rgba(255, 255, 255, 0.5);
  backdrop-filter: blur(20px);
}
</style>
