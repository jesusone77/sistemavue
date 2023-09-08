<template>
    <div id="MenuLateral">
        <v-list-item>
          <v-list-item-content>
            <v-list-item-title class="text-h6">
              MEVN
            </v-list-item-title>
            <v-list-item-subtitle>
              practice CRUD
            </v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>
        <v-divider></v-divider>
        <v-list nav>
          <v-list-item
            v-for="item in items"
            :key="item.title"
            link
          >
            <v-list-item-icon>
              <v-icon>{{ item.icon }}</v-icon>
            </v-list-item-icon>
  
            <v-list-item-content>
              <v-list-item-title>{{ item.title }}</v-list-item-title>
            </v-list-item-content>
          </v-list-item>
        </v-list>
    </div>
</template>

<script>
import 'material-design-icons-iconfont/dist/material-design-icons.css';
import axios from 'axios';
export default {
    name: '#MenuLateral',
    data () {
        return {
            categotias:[],

      items: [
        { title: 'Dashboard', icon: 'mdi-favorite' },
        { title: 'Vendedores', icon: 'mdi-image' },
        { title: 'Ventas', icon: 'mdi-help-box' },
        { title: 'Operador', icon: 'mdi-help-box' },
        { title: 'About', icon: 'mdi-help-box' },
      ],
      right: null,
    }
  },
  methods: {
    listar() {
        axios.get('http://localhost:3000/api/categoria/list').then(function (responde) {
            console.log(response);
        }).catch(function(error) {
           console.log(error);
        });
    }
  }
};
</script>

<style>

</style>