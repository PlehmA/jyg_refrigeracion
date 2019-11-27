<template>
  <v-app light>
     <v-toolbar color="brown lighten-3">
                <v-toolbar-title v-text="title" class="white--text"></v-toolbar-title>
                <v-spacer></v-spacer>
                   <v-btn to="/" class="white--text" text small>Home</v-btn>
                   <v-btn to="/contact" class="white--text" text small>Contacto</v-btn>
            </v-toolbar>
    <v-content>
      <router-view></router-view>
    </v-content>
  </v-app>
</template>

<script>
export default {
  name: 'App',
  data () {
    return {
      title: 'J&G Refrigeración'
    }
  }
}
</script>
