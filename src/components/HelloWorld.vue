<template>
  <v-app id="inspire">
    <v-navigation-drawer
      v-model="drawer"
      app
      
    >
        <v-app-bar 
    app
    flat
    color="transparent"
    > 
      <v-spacer></v-spacer>
      <v-app-bar-nav-icon @click="drawer = !drawer"  ></v-app-bar-nav-icon>

      <v-toolbar-title></v-toolbar-title>
    </v-app-bar>
      <v-list-item>
        <v-list-item-content>
          <v-list-item-title class="text-h6">
            R
          </v-list-item-title>
        </v-list-item-content>
      </v-list-item>

      <v-list
        dense
        nav
      >
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
    </v-navigation-drawer>

    <v-app-bar 
    app
    flat
    > 
      <v-spacer></v-spacer>
      <v-app-bar-nav-icon @click="drawer = !drawer"  ></v-app-bar-nav-icon>

      <v-toolbar-title></v-toolbar-title>
    </v-app-bar>

    <v-main>
      <!--  -->
    </v-main>
  </v-app>
</template>

<script>
  export default {
    name: 'HelloWorld',

    data: () => ({
      drawer: null,
       items: [
          { title: 'INICIO', icon: 'mdi-view-dashboard' },
          { title: 'SERVICIOS', icon: 'mdi-image' },
          { title: 'NUESTRO EQUIPO', icon: 'mdi-help-box' },
          { title: 'PORTAFOLIO', icon: 'mdi-help-box' },
          { title: 'CONTÁCTO', icon: 'mdi-help-box' },
          { title: 'TÉRMINOS Y CONDICIONES', icon: 'mdi-help-box' },
        ],
        right: null,
      }),
  }
</script>
