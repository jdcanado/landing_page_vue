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
          <v-list-tile @click="$vuetify.goTo('#sobre');">
            <v-list-tile-action> <v-icon>settings</v-icon> </v-list-tile-action>
            <v-list-tile-content> PRODUTOS </v-list-tile-content>
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
          <v-btn @click="$vuetify.goTo('#sobre');" flat>Produtos</v-btn>
        </v-toolbar-items>
      </v-toolbar>
      <v-content><Home /><Sobre /></v-content>
      <v-footer class="elevation-12" app>
        <span style="margin-left: 20px">JDCanado&copy; 2019</span>
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
    pagina: "Home"
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
