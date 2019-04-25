<template>
  <div app>
    <v-container id="produtos" grid-list-md text-xs-center fill-height>
      <v-layout row wrap>
        <v-flex xs12>
          <v-card>
            <v-card-title class="headline mb-0">Produtos</v-card-title>
            <v-divider/>
            <v-card-text>{{ produto }}</v-card-text>
            <v-container fluid grid-list-sm>
              <v-layout row wrap>
                <v-flex v-for="i in 6" :key="i" xs4>
                  <img
                    :src="`https://cdn.staticaly.com/gh/jdcanado/landing_page_vue/d927b924/src/assets/produtos_${i}.jpg`"
                    class="image"
                    alt="lorem"
                    width="100%"
                    height="100%"
                  >
                  
                </v-flex>
              </v-layout>
            </v-container>
            <v-card-actions>
              <v-spacer></v-spacer>
              <v-btn icon>
                <v-icon>favorite</v-icon>
              </v-btn>
              <v-btn icon>
                <v-icon>bookmark</v-icon>
              </v-btn>
              <v-btn icon>
                <v-icon>share</v-icon>
              </v-btn>
            </v-card-actions>
          </v-card>
        </v-flex>
      </v-layout>
    </v-container>
  </div>
</template>
<script>
export default {
  data() {
    return {
      produto:
        "Trabalhamos com os mais diversos segmentos da reposição de Autopeças da Linha Pesada. De acordo com a necessidade do cliente, nosso compromisso é buscar o melhor produto para atender sua demanda."
    };
  },
  name: "Produtos"
};
</script>
