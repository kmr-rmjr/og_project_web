<template>
  <v-app>
    <v-main>
      <main-page></main-page>
    </v-main>
    <v-footer color="#3D3D3D" class="py-4">
      <p class="white--text text-center ma-auto">Copyright OGATA PROJECT 2020.<br>All Rights Reserved.</p>
    </v-footer>
  </v-app>
</template>

<script>
import MainPage from './components/pages/MainPage.vue';

export default {
  name: 'App',
  components: {
    MainPage,
  },
}
</script>
