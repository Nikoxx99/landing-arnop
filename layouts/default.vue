<template>
  <v-app dark class="app-bg">
    <v-main>
      <Nuxt />
    </v-main>
    <v-footer
      :absolute="!fixed"
      app
      class="text-center justify-center"
    >
      <span>&copy; {{ new Date().getFullYear() }} ARNOProducciones S.A.S. - Todos los derechos reservados - Desarrollado con tecnologias modernas de la web</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  name: 'DefaultLayout',
  data () {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire'
        }
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js'
    }
  },
  head () {
    return {
      title: 'ARNOProducciones S.A.S.',
      meta: [
        {
          name: 'description',
          content: 'Internet en Mariquita ilimitado'
        },
        {
          name: 'keywords',
          content: 'Internet, Mariquita, Tolima, Ilimitado, Fibra optica'
        }
      ]
    }
  },
  destroyed () {
    window.removeEventListener('resize', this.isDesktopScreen)
  },
  mounted () {
    window.addEventListener('resize', this.isDesktopScreen)
    this.isDesktopScreen()
  },
  methods: {
    isDesktopScreen () {
      const res = document.body.clientWidth
      if (res < 960) {
        this.isDesktop = false
      } else {
        this.isDesktop = true
      }
      this.$store.commit('isDesktop', this.isDesktop)
    }
  }
}
</script>
<style scoped>
.app-bg {
  background-color: #ebeefb;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 1600 900'%3E%3Cdefs%3E%3ClinearGradient id='a' x1='0' x2='0' y1='1' y2='0'%3E%3Cstop offset='0' stop-color='%230FF'/%3E%3Cstop offset='1' stop-color='%23CF6'/%3E%3C/linearGradient%3E%3ClinearGradient id='b' x1='0' x2='0' y1='0' y2='1'%3E%3Cstop offset='0' stop-color='%23F00'/%3E%3Cstop offset='1' stop-color='%23FC0'/%3E%3C/linearGradient%3E%3C/defs%3E%3Cg fill='%23FFF' fill-opacity='0' stroke-miterlimit='10'%3E%3Cg stroke='url(%23a)' stroke-width='2'%3E%3Cpath transform='translate(0 0)' d='M1409 581 1450.35 511 1490 581z'/%3E%3Ccircle stroke-width='4' transform='rotate(0 800 450)' cx='500' cy='100' r='40'/%3E%3Cpath transform='translate(0 0)' d='M400.86 735.5h-83.73c0-23.12 18.74-41.87 41.87-41.87S400.86 712.38 400.86 735.5z'/%3E%3C/g%3E%3Cg stroke='url(%23b)' stroke-width='4'%3E%3Cpath transform='translate(0 0)' d='M149.8 345.2 118.4 389.8 149.8 434.4 181.2 389.8z'/%3E%3Crect stroke-width='8' transform='rotate(0 1089 759)' x='1039' y='709' width='100' height='100'/%3E%3Cpath transform='rotate(0 1400 132)' d='M1426.8 132.4 1405.7 168.8 1363.7 168.8 1342.7 132.4 1363.7 96 1405.7 96z'/%3E%3C/g%3E%3C/g%3E%3C/svg%3E");
  background-attachment: fixed;
  background-size: cover;
}
</style>
