<template>
  <div app>
    <v-container id="portfolio" grid-list-md text-xs-center fill-height>
      <v-layout row wrap>
        <v-flex xs12>
          <v-card>
            <v-card-title class="headline mb-0">Portfólio</v-card-title>
          </v-card>
        </v-flex>
        <v-flex xs12 sm4>
          <v-card>
            <v-card-title class="headline mb-0">Gestão Com. / Representação</v-card-title>
            <v-divider/>
            <v-card-text class="mb-5">{{ gestao_comercial }}</v-card-text>
            <v-img
              class="pt-3"
              src="https://cdn.staticaly.com/gh/jdcanado/landing_page_vue/46e2970b/src/assets/representacao1.png"
              aspect-ratio="1.75"
            ></v-img>

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

        <v-flex xs12 sm4>
          <v-card>
            <v-card-title class="headline mb-0">Distribuição</v-card-title>
            <v-divider/>
            <v-card-text>{{ distribuicao }}</v-card-text>
            <v-img
              src="https://cdn.staticaly.com/gh/jdcanado/landing_page_vue/46e2970b/src/assets/distribuicao1.jpg"
              aspect-ratio="1.75"
            ></v-img>

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

        <v-flex xs12 sm4>
          <v-card>
            <v-card-title class="headline mb-0">Transportadoras / Frotistas</v-card-title>
            <v-divider/>
            <v-card-text>{{ transportadoras_frotistas }}</v-card-text>
            <v-img
              src="https://cdn.staticaly.com/gh/jdcanado/landing_page_vue/46e2970b/src/assets/distribuicao3.jpg"
              aspect-ratio="1.75"
            ></v-img>

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
      gestao_comercial:
        "Cuidamos de todo o processo de venda dos produtos de nossos parceiros, sendo esses oferecidos diretamente ao mercado, reduzindo custos de manutenção da equipe comercial em regiões pré-determinadas pelos clientes.",
      distribuicao:
        "O grande diferencial da CONFIA TRUCK PARTS é o centro de armazenamento oferecido aos parceiros. Por estar situada em uma região estratégica (divisa com os estados de Minas Gerais e Mato Grosso do Sul) os clientes podem se beneficiar dessa estrutura para fixar um ponto de apoio ou mesmo redespacho de seus produtos, otimizando a logística e minimizando os custos gerados pela entrega.",
      transportadoras_frotistas:
        "Entendemos que muitos frotistas e transportadoras são quem mais “sofrem” com o mercado de reposição de Autopeças. Buscando evitar a formação de estoques próprios, temos condições especiais de parcerias para otimizar o consumo de empresas desse segmento. Resultando em agilidade e baixo custo das manutenções. Afinal, caminhão parado é dinheiro perdido!"
    };
  },
  name: "Portfolio"
};
</script>
