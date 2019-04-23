<template>
  <div app>
    <v-container id="sobre" grid-list-md text-xs-center fill-height>
      <v-layout row wrap>
        <v-flex xs12>
          <v-card>
            <v-card-title class="headline mb-0">Sobre</v-card-title>
          </v-card>
        </v-flex>
        <v-flex xs12 sm4>
          <v-card>
            <v-card-title class="headline mb-0">A Empresa</v-card-title>
            <v-divider/>
            <v-card-text>{{ empresa }}</v-card-text>
            <v-img
              src="https://cdn.staticaly.com/gh/jdcanado/landing_page_vue/46e2970b/src/assets/empresa2.jpg"
              aspect-ratio="2.75"
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
            <v-card-title class="headline mb-0">Missão</v-card-title>
            <v-divider/>
            <v-card-text class="mb-5">{{ missao }}</v-card-text>
            <v-img
              class="pt-5"
              src="https://cdn.staticaly.com/gh/jdcanado/landing_page_vue/46e2970b/src/assets/missao1.jpg"
              aspect-ratio="2.6"
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
            <v-card-title class="headline mb-0">Objetivo</v-card-title>
            <v-divider/>
            <v-card-text class="mb-5">{{ objetivo }}</v-card-text>
            <v-img
              class="pt-5"
              src="https://cdn.staticaly.com/gh/jdcanado/landing_page_vue/46e2970b/src/assets/objetivos1.jpg"
              aspect-ratio="1.8"
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
      empresa:
        "Somos uma AUTOPEÇA que nasceu de uma paixão: o CAMINHÃO. Sabemos como é difícil manter um caminhão transitando diante do alto custo de peças e das condições das estradas do país. As consequências são mais manutenção, mais tempo nas rodovias e menos qualidade de vida para o motorista e sua família. Foi pensando nisso, que nasceu a CONFIA TRUCK PARTS! Uma empresa que visa atender a necessidade deste mercado de maneira mais eficaz e com agilidade no processo de reparo do veículo, através de novas plataformas de negócios. Sempre visando o melhor custo benefício para o mercado que atende esse público. Tudo isso refletindo no bem-estar do caminhoneiro.",
      missao:
        "A CONFIA TRUCK PARTS visa atender o consumo de reposição de Autopeças da Linha Pesada com a mesma paixão que temos pelos caminhões. Oferecer peças de alta qualidade, com garantia e primando pela satisfação de nossos clientes e parceiros, sejam ele revendedores ou consumidores finais. Nossa relação com o mercado vai além do ato de comprar e vender, prezamos pelo bem-estar, pela ética e pela transparência.",
      objetivo:
        "Ser referência no mercado de AUTOPEÇAS, com reconhecimento de toda cadeia consumidora pela excelência do serviço prestado, desde a necessidade do cliente até a entrega dos produtos ao consumidor final. Nosso principal objetivo é a satisfação dos nossos clientes."
    };
  },
  name: "Sobre"
};
</script>
