<template>
  <div app>
    <v-container id="faleConosco" grid-list-md text-xs-center fill-height>
      <v-layout row wrap>
        <v-flex xs12>
          <v-card>
            <v-card-title class="headline mb-0">Fale Conosco</v-card-title>
          </v-card>
        </v-flex>
        <v-flex xs12 sm6>
          <v-card height="450">
            <v-card-title class="headline mb-0">Deixe sua mensagem</v-card-title>
            <v-divider/>
            <v-card-text>
              <v-container grid-list-md>
                <v-layout wrap>
                  <v-flex xs12 sm6>
                    <v-text-field label="Nome*" required></v-text-field>
                  </v-flex>
                  <v-flex xs12 sm6>
                    <v-text-field label="Email*" required></v-text-field>
                  </v-flex>
                  <v-flex xs12 sm12>
                    <v-textarea
                      name="msgDlg"
                      label="Mensagem*"
                      hint="Deixe sua mensagem"
                      rows="3"
                      required
                    ></v-textarea>
                  </v-flex>
                </v-layout>
              </v-container>
            </v-card-text>
            <v-card-actions>
              <v-spacer></v-spacer>
              <v-btn color="indigo" flat @click="dialog = false;">Enviar
                <v-icon left dark>send</v-icon>
              </v-btn>
            </v-card-actions>
          </v-card>
        </v-flex>

        <v-flex xs12 sm6>
          <v-card height="450">
            <v-card-title class="headline mb-0">Contato</v-card-title>
            <v-divider/>
            <v-card-text>
              <v-container grid-list-md>
                <v-layout column>
                  <v-flex xs12 sm12>
                    <v-list one-line>
                      <v-list-tile>
                        <v-list-tile-action>
                          <v-icon color="indigo">phone</v-icon>
                        </v-list-tile-action>

                        <v-list-tile-content>
                          <v-list-tile-title>(17) 99198-8261</v-list-tile-title>
                          <v-list-tile-sub-title>Celular/WhatsApp</v-list-tile-sub-title>
                        </v-list-tile-content>
                      </v-list-tile>
                      <v-list-tile>
                        <v-list-tile-action></v-list-tile-action>
                        <v-list-tile-content>
                          <v-list-tile-title>(17) 99198-8261</v-list-tile-title>
                          <v-list-tile-sub-title>Telefone</v-list-tile-sub-title>
                        </v-list-tile-content>
                      </v-list-tile>

                      <v-divider inset class="mb-3"/>

                      <v-list-tile>
                        <v-list-tile-action>
                          <v-icon color="indigo">mail</v-icon>
                        </v-list-tile-action>

                        <v-list-tile-content>
                          <v-list-tile-title>contato@confiatruckparts.com.br</v-list-tile-title>
                          <v-list-tile-sub-title>Email Corporativo</v-list-tile-sub-title>
                        </v-list-tile-content>
                      </v-list-tile>

                      <v-divider inset class="mb-3"/>

                      <v-list-tile>
                        <v-list-tile-action>
                          <v-icon color="indigo">location_on</v-icon>
                        </v-list-tile-action>

                        <v-list-tile-content>
                          <v-list-tile-title>Endereço</v-list-tile-title>
                          <v-list-tile-sub-title>Cidade</v-list-tile-sub-title>
                        </v-list-tile-content>
                      </v-list-tile>

                      <v-list-tile>
                        <v-list-tile-action/>
                        <v-list-tile-content>
                          <v-list-tile-title>Endereço</v-list-tile-title>
                          <v-list-tile-sub-title>Brasil</v-list-tile-sub-title>
                        </v-list-tile-content>
                      </v-list-tile>
                    </v-list>
                  </v-flex>
                </v-layout>
              </v-container>
            </v-card-text>
          </v-card>
        </v-flex>
      </v-layout>
    </v-container>
  </div>
</template>
