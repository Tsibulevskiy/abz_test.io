<template>
  <v-app>
    <v-navigation-drawer app absolute bottom temporary>
      <app-navigation/>
    </v-navigation-drawer>
    <v-app-bar app>
      <app-header/>
    </v-app-bar>
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
import appNavigation from "@/components/appNavigation"

export default {
  components: {
    appMain,
    appFooter,
    appHeader,
    appNavigation
  }
}
</script>
