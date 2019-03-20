<template>
  <div app>
    <v-container id="portfolio" grid-list-md text-xs-center fill-height>
      <v-layout row wrap>
        <v-flex xs12>
          <v-card>
            <v-card-title class="headline mb-0">Contato</v-card-title>
          </v-card>
        </v-flex>
        <v-flex xs12 sm6>
          <v-card>
            <v-card-title class="headline mb-0">Deixe sua mensagem</v-card-title>
            <v-divider/>
            <v-card-text>
              <v-container grid-list-md>
                <v-layout wrap>
                  <v-flex xs12 sm4>
                    <v-text-field label="Nome*" required></v-text-field>
                  </v-flex>
                  <v-flex xs12 sm4>
                    <v-text-field label="Sobrenome*" required></v-text-field>
                  </v-flex>
                  <v-flex xs12 sm4>
                    <v-text-field label="Email*" required></v-text-field>
                  </v-flex>
                </v-layout>
              </v-container>
            </v-card-text>
            <v-card-actions>
              <v-spacer></v-spacer>
              <v-btn color="blue darken-1" flat @click="dialog = false;">Enviar
                <v-icon left dark>send</v-icon>
              </v-btn>
            </v-card-actions>
          </v-card>
        </v-flex>

        <v-flex xs12 sm6>
          <v-card>
            <v-card-title class="headline mb-0">Fale conosco</v-card-title>
            <v-divider/>
            <v-card-text>
              <v-container grid-list-md>
                <v-layout wrap></v-layout>
              </v-container>
            </v-card-text>
          </v-card>
        </v-flex>
      </v-layout>
    </v-container>
  </div>
</template>
