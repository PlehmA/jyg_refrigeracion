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
      <v-footer color="brown lighten-3">
                    <v-layout row wrap align-center>
                        <v-flex xs12>
                            <div class="white--text ml-4">
                                Made with
                                <img src="./assets/images/como.svg" alt="" class="love_image">
                                by <a class="white--text" href="https://styleprog.tech" target="_blank">StyleProg</a> &copy; All rights reserved
                            </div>
                        </v-flex>
                    </v-layout>
                </v-footer>
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

<style>
.love_image{
height: 24px;
}
</style>
