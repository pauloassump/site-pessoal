<template>
  <v-app>
    <Header />
    <v-main class="main">
      <v-container fluid>
        <router-view></router-view>
        <Footer />
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
import Header from '@/components/Header'
import Footer from '@/components/Footer'

export default {
  name: 'App',

  components: {
    Header,
    Footer
  },

  data: () => ({
    //
  }),
};
</script>

<style>
.v-main {
  background-color: #34495f;
}
</style>
