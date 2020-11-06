<template>
<v-card flat color="#3ab982">
  <h2 class="text-center">Linha do Tempo</h2>
  <v-timeline
    align-top
    :dense="$vuetify.breakpoint.smAndDown"
  >
    <v-timeline-item
      fill-dot
      icon="mdi-briefcase"
    >
      <template v-slot:opposite>
        <span
          class="headline font-weight-bold black--text"
        >01/07/2020</span>
      </template>
      <v-card
        dark
        color="#34495f"
      >
        <v-card-title class="title">
          Ponto Sistemas
        </v-card-title>
        <v-card-text class="white text--primary">
          <p>-Desenvolvimento Frontend utilizando Nuxtjs e Vuetify.</p>
        </v-card-text>
      </v-card>
    </v-timeline-item>

    <v-timeline-item
      fill-dot
      icon="mdi-briefcase"
    >
      <template v-slot:opposite>
        <span
          class="headline font-weight-bold black--text"
        >01/11/2019 à 01/06/2020</span>
      </template>
      <v-card
        dark
        color="#34495f"
      >
        <v-card-title class="title">
          Agapys Tecnologia
        </v-card-title>
        <v-card-text class="white text--primary">
          <p>- Desenvolvimento front-end utilizando HTML, CSS, JavaScript e VueJs.</p>
          <p>- Criação de componentes em VueJS para atender as demandas.</p>
        </v-card-text>
      </v-card>
    </v-timeline-item>

    <v-timeline-item
      fill-dot
      icon="mdi-briefcase"
    >
      <template v-slot:opposite>
        <span
          class="headline font-weight-bold black--text"
          >01/06/2016 à 20/10/2019</span>
      </template>
      <v-card
        dark
        color="#34495f"
      >
        <v-card-title class="title">
          Ambiental Limpeza Urbana e Saneamento LTDA
        </v-card-title>
        <v-card-text class="white text--primary">
          <p>- Suporte técnico ao usuário priorizando e discernindo chamados</p>
          <p>- Administração da rede gerenciando as permissões de usuários e regras do Firewall</p>
          <p>- Identificar problemas de Hardware e Software</p>
          <p>- Gerenciar as permissões de usuários dos servidores Samba</p>
          <p>- Manutenção e conservação de equipamentos de informática</p>
          <p>- Rotinas de backup</p>
          <p>- Identificar soluções e melhorias para o departamento de TI</p>
          <p>- Classificação de notas fiscais</p>
        </v-card-text>
      </v-card>
    </v-timeline-item>

  </v-timeline>
</v-card>
</template>

<script>
  export default {
    data: () => ({
      items: [
        {
          color: 'red lighten-2',
          icon: 'mdi-star',
        },
        {
          color: 'purple darken-1',
          icon: 'mdi-book-variant',
        },
        {
          color: 'green lighten-1',
          icon: 'mdi-airballoon',
        },
        {
          color: 'indigo',
          icon: 'mdi-buffer',
        },
      ],
    }),
  }
</script>