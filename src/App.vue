<template>
  <v-app>
    <v-navigation-drawer temporary v-model="sideNav" absolute>
      <v-list>

      </v-list>
    </v-navigation-drawer>
    <v-toolbar dark class="indigo darken-4">
      <v-toolbar-side-icon @click.native.stop= "sideNav = !sideNav"></v-toolbar-side-icon>
      <v-toolbar-title>GoGo car</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-toolbar-items>
       <v-btn flat>
         <v-icon left>question_answer</v-icon>
         TARIFF
       </v-btn>
       <v-btn flat>
         <v-icon left>lock_open</v-icon>
         SIGNUP
       </v-btn>
       <v-btn flat>
         <v-icon left>face</v-icon>
         LOGIN
       </v-btn>
     </v-toolbar-items>
   </v-toolbar>
  </v-app>
</template>

<script>
export default {
  data () {
    return {
      sideNav: false
    }
  },
  name: 'App'
}
</script>
