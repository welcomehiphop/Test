<template>
  <v-app-bar app dark>
    <div class="d-flex align-center">
      <v-btn href="/home" text>
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-logo-dark.png"
          transition="scale-transition"
          width="40"
        />
        <v-img
          alt="Vuetify Name"
          class="shrink mt-1 hidden-sm-and-down"
          contain
          min-width="40"
          src="../assets/logo.png"
          width="50"
        />
      </v-btn>
    </div>
    <v-spacer></v-spacer>
    <v-btn href="" text>
      <span class="mr-2">Latest Release</span>
      <v-icon>mdi-open-in-new</v-icon>
    </v-btn>
    
  </v-app-bar>
</template>

<script>
export default {};
</script>

<style></style>
