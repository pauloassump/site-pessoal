<template>
  <v-row>
    <v-col cols="12" md="12">
      <v-card flat>
        <v-img
          height="200px"
          src="https://cdn-images-1.medium.com/fit/t/1600/480/1*vFC8tDUGLlXIiqT7ymf3xg.png"
        >
          <v-card-title class="white--text mt-8">
            <v-avatar size="66">
              <img
                alt="user"
                src="https://media-exp1.licdn.com/dms/image/C4E03AQH6gwFRRFdOlQ/profile-displayphoto-shrink_200_200/0?e=1609977600&v=beta&t=ep0kl052RmPSOYaVnvZru_qb4V6jRxRlGHZh61Ih0ZU"
              >
            </v-avatar>
            
            <br />
          </v-card-title>
          <p class="white--text ml-2">
            <strong>Paulo Henrique de Assumpção</strong>
            <p class="white--text ml-2">Desenvolvedor Vuejs</p>
        </v-img>
      </v-card>
    </v-col>

    <v-col cols="12" md="6">
      <Perfil />
    </v-col>

    <v-col cols="12" md="6">
      <Profissional />
    </v-col>

    <!-- <v-col cols="12" md="4">
      <Frase />
    </v-col> -->
    
    <v-col cols="12" md="12">
      <Timeline />
    </v-col>

  </v-row>
</template>

<script>
import Perfil from '@/components/Perfil'
import Profissional from '@/components/Profissional'
// import Frase from '@/components/Frase'
import Timeline from '@/components/Timeline'

export default {
  components: {
    Perfil,
    Profissional,
    Timeline
  }
}
</script>

<style>

</style>