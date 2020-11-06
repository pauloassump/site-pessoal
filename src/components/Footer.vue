<template>
  <v-card color="#34495f" flat height="200px">
    <v-footer
      v-bind="localAttrs"
      color="#34495f"
    >
      <v-card
        flat
        tile
        width="100%"
        class="text-center"
        color="#3ab982"
      >
      <v-card-text class="white--text">
          <strong>Onde você pode me encontrar?</strong>
        </v-card-text>
        <v-card-text>
          <v-btn
            class="mx-4"
            icon
          >
          <a href="https://www.linkedin.com/in/paulohenriquedeassumpcao/">
            <v-icon size="35px">
              mdi-linkedin
            </v-icon>
          </a>
          </v-btn>

          <v-btn
            class="mx-4"
            icon
          >
          <a href="mailto:paulo.henriquejcn@gmail.com">
            <v-icon size="35px">
              mdi-email
            </v-icon>
          </a>
          </v-btn>

          <v-btn
            class="mx-4"
            icon
          >
          <a href="https://www.instagram.com/paulo.henass">
            <v-icon size="35px">
              mdi-instagram
            </v-icon>
          </a>
          </v-btn>
        </v-card-text>

        <v-divider></v-divider>

        <v-card-text class="white--text">
          {{ new Date().getFullYear() }} — <strong>Desenvolvido por Paulo Henrique de Assumpção</strong>
        </v-card-text>
      </v-card>
    </v-footer>

    <v-row
      align="center"
      justify="center"
      class="ma-12"
    >
      <v-col
        cols="12"
        md="8"
      >
      </v-col>
    </v-row>
  </v-card>
</template>

<script>
  export default {
    data: () => ({
      icons: [
        'mdi-linkedin',
        'mdi-email',
        'mdi-instagram',
        'mdi-facebook',
      ],
      padless: false,
      variant: 'absolute',
    }),
    computed: {
      localAttrs () {
        const attrs = {}

        if (this.variant === 'default') {
          attrs.absolute = false
          attrs.fixed = false
        } else {
          attrs[this.variant] = true
        }
        return attrs
      },
    },
  }
</script>

<style>
a:link {
  text-decoration: none;
}
</style>