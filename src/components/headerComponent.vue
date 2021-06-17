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
         :to="item.url">
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
    name: 'headerComponent',

    data: () => ({
      drawer: null,
       items: [
          { title: 'INICIO', icon: 'mdi-view-dashboard', url:'home' },
          { title: 'SERVICIOS', icon: 'mdi-image', url:'servicios' },
          { title: 'NUESTRO EQUIPO', icon: 'mdi-help-box', url:'nuestroequipo' },
          { title: 'PORTAFOLIO', icon: 'mdi-help-box', url:'portafolio' },
          { title: 'CONTÁCTO', icon: 'mdi-help-box', url:'contacto' },
          { title: 'TÉRMINOS Y CONDICIONES', icon: 'mdi-help-box', url:'terminos' },
        ],
        right: null,
      }),
  }
</script>
