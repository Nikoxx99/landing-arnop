<template>
  <v-img
    src="hero.png"
    :height="$store.state.isDesktop ? '100vh' : '60vh'"
    cover
  >
    <div v-if="$store.state.isDesktop" style="position:absolute;display:grid;place-items:center;height:100%;width:100%;">
      <div
        class="elevation-10"
        style="margin-left:30%;display:block;text-align:end;justify-content:end;padding:20px;backdrop-filter:blur(20px);background-color:rgba(255,255,255,.07);border-radius:20px;"
      >
        <MiscLogoArnop />
        <h1 class="text-h5">
          <strong>Internet ilimitado en Mariquita y Fresno</strong>
        </h1>
        <h2 class="font-weight-regular font-italic">
          Porque ya somos parte de tu hogar
        </h2>
      </div>
    </div>
    <div v-else style="display:grid;place-items:center;height:100%;width:100%;">
      <div
        class="elevation-10"
        style="display:grid;place-items:center;text-align:center;padding:20px;backdrop-filter:blur(20px);background-color:rgba(255,255,255,.07);border-radius:20px;width:80%;"
      >
        <MiscLogoArnop />
        <h1 class="text-h5">
          <strong>Internet ilimitado en Mariquita y Fresno</strong>
        </h1>
        <h2 class="font-weight-regular font-italic">
          Porque ya somos parte de tu hogar
        </h2>
      </div>
    </div>
  </v-img>
</template>
