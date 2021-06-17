<style scoped>
  .main-letter{
    font-size: 120px;
    font-weight: bold;
    color: white;
  }
  .main {
    /* bg */
    background: #393FD0;
    justify-content: center;
    text-align:center
  }

   .fill13 {
    position: absolute;
left: 12.8%;
right: 23.38%;
top: -11.4%;
bottom: 71.04%;
}

.fill17{
  position: absolute;
left: 77.07%;
right: 60.66%;
top: 29.31%;
bottom: 37.71%;
}

.fill8{
  position: absolute;
left: -17.07%;
right: 45.66%;
top: 29.31%;
bottom: 37.71%;

}

.logo{
  position: absolute;
left: 37.87%;
right: 37.71%;
top: 7.76%;
bottom: 74.16%;

}

  .logo-main{
    background-color: rgba(76, 175, 80, 0)
  }

  .login-content-tab{
    width: 80%; 
    margin: 0 auto;
    margin-top: 250px;
  }
</style>

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

    <v-main class="main">

        <svg class="fill13" width="240" height="236" viewBox="0 0 240 236" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path opacity="0.57" fill-rule="evenodd" clip-rule="evenodd" d="M191.469 -52V119.956L0 -52V20.5237L239.314 235.176V234.832V234.458V-52H191.469Z" fill="#3B2059"/>
        </svg>
        <svg class="fill8" width="204" height="268" viewBox="0 0 204 268" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path opacity="0.523324" fill-rule="evenodd" clip-rule="evenodd" d="M203.777 267.777H153.903L131.826 223.275H181.352L203.777 267.777ZM8.29937 222.913L-14.4608 267.777H-64L69.8955 0L159.275 178.732H109.038L69.8955 100.069L30.3757 178.732L8.29937 222.913Z" fill="#3B2059"/>
        </svg>
        <svg class="fill17" width="105" height="330" viewBox="0 0 105 330" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path opacity="0.458277" fill-rule="evenodd" clip-rule="evenodd" d="M166.47 274.857C151.11 274.857 136.995 271.977 123.279 266.611C110.011 260.866 98.3708 253.047 88.4241 242.759C78.0457 232.867 70.1581 221.361 64.3462 208.192C58.5177 194.612 55.6117 180.621 55.6117 165.395C55.6117 150.153 58.5177 136.178 64.3462 122.581C70.1581 109.413 78.0457 97.907 88.4241 88.0143C98.3708 77.7265 110.011 69.9077 123.279 64.163C136.995 58.8133 151.11 55.9163 166.47 55.9163C196.343 55.9163 222.497 66.2041 244.499 87.6192L283.953 49.3321C268.577 34.1226 250.743 22.1723 230.816 13.5305C230.567 13.4318 230.301 13.3659 230.069 13.2507L230.799 12.7733C210.889 4.13158 189.286 0 166.47 0C143.621 0 122.05 4.52664 102.107 13.1684C81.7653 21.8102 64.3628 33.744 48.9695 48.5585C34.6556 63.1589 23.0982 79.6853 14.48 98.7794C14.098 99.6024 13.6331 100.36 13.2678 101.183C12.0224 104.096 11.0426 107.092 9.94668 110.055C3.52036 127.519 0 145.593 0 164.621C0 164.753 0.0166055 164.885 0.0166055 165.016C0.0166055 165.132 0 165.263 0 165.395C0 188.028 4.5665 209.41 13.2678 229.591C22.0022 249.344 34.0246 266.611 48.9695 281.442C64.3462 296.651 81.7819 308.173 102.107 316.832C122.034 325.473 143.637 330 166.47 330C189.302 330 210.889 325.868 230.816 317.243C250.743 308.601 268.577 296.651 283.953 281.442L244.499 243.154C222.497 264.57 196.343 274.857 166.47 274.857Z" fill="#3B2059"/>
        </svg>

        <!-- <div>
          <h1 class="main-letter">
            R
          </h1>
        </div> -->

        <svg class="logo" width="92" height="147" viewBox="0 0 92 147" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path d="M0 139.2V6.79999C0 4.93333 0.666666 3.33333 2 2C3.33333 0.666664 5 0 7 0H45C75.6667 0 91 13.6 91 40.8C91 52.1333 88.4667 61.0667 83.4 67.6C78.3333 74 71.4667 78.2667 62.8 80.4L90.8 133C91.3333 133.933 91.6 134.933 91.6 136C91.6 138.667 90.2 141.133 87.4 143.4C84.7333 145.667 81.8667 146.8 78.8 146.8C75.3333 146.8 72.5333 144.733 70.4 140.6L41.2 83.4H21V139.2C21 141.333 19.9333 143.067 17.8 144.4C15.8 145.6 13.3333 146.2 10.4 146.2C7.6 146.2 5.13333 145.6 3 144.4C1 143.067 0 141.333 0 139.2ZM21 66.4H45C61.5333 66.4 69.8 58.4667 69.8 42.6C69.8 26.7333 61.5333 18.8 45 18.8H21V66.4Z" fill="white"/>
        </svg>
        

      <v-card class="login-content-tab">
      <v-tabs>
        <v-tab>Log in</v-tab>
        <v-tab>Register</v-tab>
      </v-tabs>
    </v-card>
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
