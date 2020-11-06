<template>
  <div>
    <v-card color="#3ab982">
      <v-card-title class="white--text">Um pouco sobre mim...</v-card-title>
      <v-card-text class="white--text">
        Tenho 29 anos, comecei na área de TI como suporte. Foi uma porta de entrada para a area de TI, mas sempre sonhei em trabalhar com desenvolvimento...
      </v-card-text>
      <v-card-actions>
        <v-btn text @click="perfilDialog = true">
          <span class="white--text">Mais</span>
        </v-btn>
      </v-card-actions>
    </v-card>
    <v-dialog v-model="perfilDialog">
      <v-card class="pa-5">
        <v-card-title>Um pouco sobre mim...</v-card-title>
        <v-card-text class="mt-5">
          Tenho 29 anos, comecei na área de TI como suporte. Foi uma porta de entrada para a area de TI, mas sempre sonhei em trabalhar com desenvolvimento, tanto front-end como back-end. Após alguns cursos e projetos que desenvolvi por conta própria, me apaixonei por front-end e javascript. A partir desse momento comecei a focar o aprendizado em VueJS, pois nesse meio tempo também consegui meu primeiro emprego como desenvolvedor Web, utilizando essa tecnologia. Ainda almejo ser um desenvolvedor full-stack, mas antes disso, meu objetivo é dominar o front-end com VueJS e javascript.
        </v-card-text>
        <v-card-actions pl-5>
          <v-btn text @click="perfilDialog = false">Fechar</v-btn>
        </v-card-actions>
      </v-card>
    </v-dialog>
  </div>
</template>

<script>

export default {
  data () {
    return {
      perfilDialog: false,
    }
  }
}
</script>

<style>

</style>