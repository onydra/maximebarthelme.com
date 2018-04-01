<template>
  <div id="app">
    <v-app dark class="base">
      <router-view/>
    </v-app>
  </div>
</template>

<style>
@font-face {
    font-family: 'BebasNeueRegular';
    src: url('../static/fonts/bebas/BebasNeueRegular.eot?#iefix') format('embedded-opentype'),  url('../static/fonts/bebas/BebasNeueRegular.otf')  format('opentype'),
           url('../static/fonts/bebas/BebasNeueRegular.woff') format('woff'), url('../static/fonts/bebas/BebasNeueRegular.ttf')  format('truetype'), url('../static/fonts/bebas/BebasNeueRegular.svg#BebasNeueRegular') format('svg');
    font-weight: normal;
    font-style: normal;
}

@font-face {
    font-family: 'BebasNeueLight';
    src: url('../static/fonts/bebas/BebasNeueLight.eot?#iefix') format('embedded-opentype'),  url('../static/fonts/bebas/BebasNeueLight.otf')  format('opentype'),
           url('../static/fonts/bebas/BebasNeueLight.woff') format('woff'), url('../static/fonts/bebas/BebasNeueLight.ttf')  format('truetype'), url('../static/fonts/bebas/BebasNeueLight.svg#BebasNeueLight') format('svg');
    font-weight: normal;
    font-style: normal;
}

html, body {
  background: #24282E;
  margin: 0;
}

h1, h2, h3, h4, h5 {
  color: white;
  font-family: 'BebasNeueRegular';
}

.font-regular {
  font-family: 'BebasNeueRegular';
}

#app {
  min-height: 100vh;
}

a {
  color: white!important;
  text-decoration: none; /* no underline */
}

</style>
