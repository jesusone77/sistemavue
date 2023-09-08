<template>
<!-- App.vue -->

<v-app>
  <v-navigation-drawer app>
    <MenuLateral></MenuLateral>
  </v-navigation-drawer>

  <v-app-bar app>
    Esto es la barra superior
  </v-app-bar>

  <!-- Sizes your content based upon application components -->
  <v-main>

    <!-- Provides the application the proper gutter -->
    <v-container fluid>

      <!-- If using vue-router -->
      <router-view></router-view>
    </v-container>
  </v-main>

  <v-footer app>
    <!-- -->
  </v-footer>
</v-app>
</template>

<script>
import MenuLateral from './components/MenuLateral.vue';
import 'material-design-icons-iconfont/dist/material-design-icons.css';
export default {

  name: 'App',

  data () {
    return {
 
    }
  },
  components: {
    MenuLateral
  },
  icons: {
    iconfont: 'mdiSvg', // 'mdi' || 'mdiSvg' || 'md' || 'fa' || 'fa4' || 'faSvg'
  },
};
</script>
