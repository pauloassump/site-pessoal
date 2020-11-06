<template>
  <div>
    <v-card color="#3ab982">
      <v-card-title class="white--text">Profissional</v-card-title>
      <v-card-text class="white--text">Atualmente trabalho com desenvolvimento Frontend utilizando as tecnologias Vuejs e Nuxt.js, criando sistemas webs responsivos com Vuetifty...</v-card-text>
      <v-card-actions>
        <v-btn text @click="profissionalDialog = true">
          <span class="white--text">Mais</span>
        </v-btn>
      </v-card-actions>
    </v-card>
    <v-dialog v-model="profissionalDialog">
      <v-card>
        <v-card-title>Profissional</v-card-title>
      <v-card-text>Atualmente trabalho com desenvolvimento Frontend utilizando as tecnologias Vuejs e Nuxt.js, criando sistemas webs responsivos com Vuetifty. Também trabalhei 4 anos como suporte técnico em TI, atendendo problemas dos usuários e administrando a rede da empresa, supervisionando a rotina de backups e aquisições de equipamentos de TI para atender as demandas do setor. </v-card-text>
      <v-card-actions>
        <v-btn text @click="profissionalDialog = false">
          <span>
            Fechar
          </span>
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
      profissionalDialog: false
    }
  }
}
</script>

<style>

</style>