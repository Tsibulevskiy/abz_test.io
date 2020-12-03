<template>
<v-container>
  <v-row>
    <v-col cols="12">
      <about/>
    </v-col>
    <v-col cols="12">
      <relationships/>
    </v-col>
    <v-col cols="12">
      <requirements/>
    </v-col>
    <v-col cols="12">
      <users/>
    </v-col>
    <v-col cols="12">
      <sign-up/>
    </v-col>
  </v-row>
</v-container>
</template>

<script>
import about from "@/components/main/about"
import relationships from "@/components/main/relationships"
import requirements from "@/components/main/requirements"
import users from "@/components/main/users"
import signUp from "@/components/main/signUp"

export default {
  components: {
    about,
    relationships,
    requirements,
    users,
    signUp
  }
}
</script>

<style scoped>

</style>
