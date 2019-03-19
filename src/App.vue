<template>
  <div id="app">
    <v-app id="inspire">
      <v-navigation-drawer clipped fixed v-model="drawer" app>
        <v-list dense>
          <v-list-tile @click="$vuetify.goTo('#home');">
            <v-list-tile-action> <v-icon>home</v-icon> </v-list-tile-action>
            <v-list-tile-content> HOME </v-list-tile-content>
          </v-list-tile>
          <v-list-tile @click="$vuetify.goTo('#sobre');">
            <v-list-tile-action>
              <v-icon>touch_app</v-icon>
            </v-list-tile-action>
            <v-list-tile-content> SOBRE </v-list-tile-content>
          </v-list-tile>
          <v-list-tile @click="$vuetify.goTo('#produtos');">
            <v-list-tile-action> <v-icon>settings</v-icon> </v-list-tile-action>
            <v-list-tile-content> PRODUTOS </v-list-tile-content>
          </v-list-tile>
          <v-list-tile @click="$vuetify.goTo('#portfolio');">
            <v-list-tile-action> <v-icon>settings</v-icon> </v-list-tile-action>
            <v-list-tile-content> PORTFÓLIO </v-list-tile-content>
          </v-list-tile>
          <v-list-tile @click="$vuetify.goTo('#contato');">
            <v-list-tile-action> <v-icon>settings</v-icon> </v-list-tile-action>
            <v-list-tile-content> CONTATO </v-list-tile-content>
          </v-list-tile>
        </v-list>
      </v-navigation-drawer>
      <v-toolbar app fixed clipped-left>
        <v-toolbar-side-icon @click.stop="drawer = !drawer;"
          ><v-icon v-if="drawer">close</v-icon></v-toolbar-side-icon
        >
        <v-toolbar-title>Layout 1</v-toolbar-title>
        <v-spacer></v-spacer>
        <v-toolbar-items class="hidden-sm-and-down">
          <v-btn @click="$vuetify.goTo('#home');" flat>Home</v-btn>
          <v-btn @click="$vuetify.goTo('#sobre');" flat>Sobre</v-btn>
          <v-btn @click="$vuetify.goTo('#produtos');" flat>Produtos</v-btn>
          <v-btn @click="$vuetify.goTo('#portfolio');" flat>Portfólio</v-btn>
          <v-btn @click="$vuetify.goTo('#contato');" flat>Contato</v-btn>
        </v-toolbar-items>
      </v-toolbar>
      <v-content
        ><Home /><Sobre /><Produtos /><Portfolio /><Contato
      /></v-content>
      <v-footer class="elevation-12" app>
        <v-layout row justify-center>
          <v-dialog v-model="dialog" persistent max-width="600px">
            <v-card>
              <v-card-title>
                <span class="headline">User Profile</span>
              </v-card-title>
              <v-card-text>
                <v-container grid-list-md>
                  <v-layout wrap>
                    <v-flex xs12 sm6 md4>
                      <v-text-field
                        label="Legal first name*"
                        required
                      ></v-text-field>
                    </v-flex>
                    <v-flex xs12 sm6 md4>
                      <v-text-field
                        label="Legal middle name"
                        hint="example of helper text only on focus"
                      ></v-text-field>
                    </v-flex>
                    <v-flex xs12 sm6 md4>
                      <v-text-field
                        label="Legal last name*"
                        hint="example of persistent helper text"
                        persistent-hint
                        required
                      ></v-text-field>
                    </v-flex>
                    <v-flex xs12>
                      <v-text-field label="Email*" required></v-text-field>
                    </v-flex>
                    <v-flex xs12>
                      <v-text-field
                        label="Password*"
                        type="password"
                        required
                      ></v-text-field>
                    </v-flex>
                    <v-flex xs12 sm6>
                      <v-select
                        :items="['0-17', '18-29', '30-54', '54+']"
                        label="Age*"
                        required
                      ></v-select>
                    </v-flex>
                    <v-flex xs12 sm6>
                      <v-autocomplete
                        :items="[
                          'Skiing',
                          'Ice hockey',
                          'Soccer',
                          'Basketball',
                          'Hockey',
                          'Reading',
                          'Writing',
                          'Coding',
                          'Basejump'
                        ]"
                        label="Interests"
                        multiple
                      ></v-autocomplete>
                    </v-flex>
                  </v-layout>
                </v-container>
                <small>*indicates required field</small>
              </v-card-text>
              <v-card-actions>
                <v-spacer></v-spacer>
                <v-btn color="blue darken-1" flat @click="dialog = false;"
                  >Close</v-btn
                >
                <v-btn color="blue darken-1" flat @click="dialog = false;"
                  >Save</v-btn
                >
              </v-card-actions>
            </v-card>
          </v-dialog>
        </v-layout>
        <span style="margin-left: 20px">JDCanado&copy; 2019</span>
        <v-btn
          color="pink"
          @click="dialog = true;"
          dark
          medium
          right
          absolute
          fab
        >
          <v-icon>add</v-icon>
        </v-btn>
      </v-footer>
    </v-app>
  </div>
</template>

<script>
import Home from "./components/Home";
import Sobre from "./components/Sobre";
import Produtos from "./components/Produtos";
import Portfolio from "./components/Portfolio";
import Contato from "./components/Contato";

export default {
  name: "App",
  components: {
    Home,
    Sobre,
    Produtos,
    Portfolio,
    Contato
  },
  data: () => ({
    drawer: false,
    pagina: "Home",
    dialog: false
  }),
  props: {
    source: String
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 0px;
}
</style>
