<template>
  <div>
    <v-row>
      <MainHeroLanding />
    </v-row>
    <v-row style="margin-top:-100px;">
      <v-container>
        <v-row>
          <v-col cols="12" md="6" lg="6" class="d-flex justify-end">
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
          <v-col cols="12" md="6" lg="6" class="d-flex justify-start">
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
      </v-container>
    </v-row>
    <v-row justify="center" align="center">
      <v-col cols="12" sm="8" md="6">
        <v-card class="logo py-4 d-flex justify-center">
          <MiscLogoArnop />
        </v-card>
        <v-card>
          <v-card-title class="headline">
            Welcome to the Vuetify + Nuxt.js template
          </v-card-title>
          <v-card-text>
            <p>Vuetify is a progressive Material Design component framework for Vue.js. It was designed to empower developers to create amazing applications.</p>
            <p>
              For more information on Vuetify, check out the <a
                href="https://vuetifyjs.com"
                target="_blank"
                rel="noopener noreferrer"
              >
                documentation
              </a>.
            </p>
            <p>
              If you have questions, please join the official <a
                href="https://chat.vuetifyjs.com/"
                target="_blank"
                rel="noopener noreferrer"
                title="chat"
              >
                discord
              </a>.
            </p>
            <p>
              Find a bug? Report it on the github <a
                href="https://github.com/vuetifyjs/vuetify/issues"
                target="_blank"
                rel="noopener noreferrer"
                title="contribute"
              >
                issue board
              </a>.
            </p>
            <p>Thank you for developing with Vuetify and I look forward to bringing more exciting features in the future.</p>
            <div class="text-xs-right">
              <em><small>&mdash; John Leider</small></em>
            </div>
            <hr class="my-3">
            <a
              href="https://nuxtjs.org/"
              target="_blank"
              rel="noopener noreferrer"
            >
              Nuxt Documentation
            </a>
            <br>
            <a
              href="https://github.com/nuxt/nuxt.js"
              target="_blank"
              rel="noopener noreferrer"
            >
              Nuxt GitHub
            </a>
          </v-card-text>
          <v-card-actions>
            <v-spacer />
            <v-btn
              color="primary"
              nuxt
              to="/inspire"
            >
              Continue
            </v-btn>
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>
  </div>
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
