<template>
  <v-app>
    <webapp-header/>
    <v-content class="heh">
      <router-view></router-view>
    </v-content>
    <webapp-footer/>
  </v-app>
</template>

<script>
import header from './components/header.vue'
import footer from './components/footer.vue'

export default {
  name: 'App',

  components: {
    'webapp-header':header,
    'webapp-footer':footer
  },

  data () {
    return {

    }
  }
}
</script>

<style>
@font-face {
font-family: "gothamB";
src: url('fonts/GothamBold.otf');
}
@font-face {
font-family: "gothamM";
src: url('fonts/GothamMedium.ttf');
}
@font-face {
font-family: "din";
src: url('fonts/DINPro-CondLight.otf');
}

.heh{
  background: rgb(255, 252, 247);
}

/* MEDIA QUERIES */
@media only screen and (min-width: 960px){
  .container {
      max-width: 1264px;
    }
}
@media only screen and (min-width: 1264px){
  .container {
      max-width: 1904px;
    }
}


</style>
