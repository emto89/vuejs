<template>
 <v-card
    class="mx-auto overflow-hidden"
  >
    <v-app-bar    
    flat  
    >
      <v-app-bar-tittle>Logo</v-app-bar-tittle>

      <v-spacer></v-spacer>
      <v-btn icon>
        <v-icon>mdi-magnify</v-icon>
      </v-btn>

      <v-btn icon>
        <v-icon>mdi-filter</v-icon>
      </v-btn>

      <v-btn icon>
        <v-icon>mdi-dots-vertical</v-icon>
      </v-btn>
    <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
    </v-app-bar>

    <v-navigation-drawer
      v-model="drawer"
      absolute
      bottom
      temporary
    >
      <v-list
        nav
        dense
      >
        <v-list-item-group
          v-model="group"
          active-class="deep-purple--text text--accent-4"
        >
          <v-list-item>
            <v-list-item-title>Foo</v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-title>Bar</v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-title>Fizz</v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-title>Buzz</v-list-item-title>
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>

    <v-card-text>
      The navigation drawer will appear from the bottom on smaller size screens.
    </v-card-text>
  </v-card>
</template>

<script>
  export default {
    name: 'indexPage',

    data: () => ({
      drawer: null,
       items: [
          { title: 'INICIO', icon: 'mdi-view-dashboard', url:'about' },
          { title: 'SERVICIOS', icon: 'mdi-image', url:'servicios' },
          { title: 'NUESTRO EQUIPO', icon: 'mdi-help-box', url:'nuestroequipo' },
          { title: 'PORTAFOLIO', icon: 'mdi-help-box', url:'portafolio' },
          { title: 'CONTÁCTO', icon: 'mdi-help-box', url:'contacto' },
          { title: 'TÉRMINOS Y CONDICIONES', icon: 'mdi-help-box', url:'terminos' },
        ],
        right: null,
      }),
      watch: {
      group () {
        this.drawer = false
      },
    },
  }
</script>