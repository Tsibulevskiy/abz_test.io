<template>
  <v-app>
    <v-app-bar app>
      <v-app-bar-nav-icon color="secondary" @click="drawer=!drawer"></v-app-bar-nav-icon>
      <app-header/>
    </v-app-bar>
    <v-navigation-drawer temporary absolute v-model="drawer"></v-navigation-drawer>
    <v-main>
      <v-container fluid>
        <app-main/>
      </v-container>
    </v-main>
    <v-footer app>
      <app-footer/>
    </v-footer>
  </v-app>
</template>

<script>
import appHeader from "@/components/appHeader"
import appFooter from "@/components/appFooter"
import appMain from "@/components/appMain"

export default {
  components: {
    appMain,
    appFooter,
    appHeader
  },
  data () {
    return {
      drawer: false
    }
  }
}
</script>
