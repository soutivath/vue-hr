<template>
  <v-app-bar absolute color="white" elevate-on-scroll app>
      <v-app-bar-nav-icon
        v-if="$vuetify.breakpoint.mdAndUp"
        class="mr-5 ml-5 mt-2"
        style="-webkit-box-shadow: -3px -3px 57px -3px rgba(0,0,0,0.33);
        -moz-box-shadow: -3px -3px 57px -3px rgba(0,0,0,0.33);
        box-shadow: -3px -3px 57px -3px rgba(0,0,0,0.33);"
        @click="displayMini=!displayMini"
      >
        <v-icon v-if="displayMini==false">mdi mdi-dots-vertical</v-icon>
      </v-app-bar-nav-icon>

      <v-toolbar-title>Dashboard</v-toolbar-title>

      <v-spacer></v-spacer>
      <v-btn icon>
        <v-icon>mdi mdi-invert-colors</v-icon>
      </v-btn>
      <v-app-bar-nav-icon
        v-if="$vuetify.breakpoint.smAndDown"
        class="mr-5 ml-5 mt-2"
        style="-webkit-box-shadow: -3px -3px 57px -3px rgba(0,0,0,0.33);
        -moz-box-shadow: -3px -3px 57px -3px rgba(0,0,0,0.33);
        box-shadow: -3px -3px 57px -3px rgba(0,0,0,0.33);"
        @click="drawer=!drawer"
      ></v-app-bar-nav-icon>
    </v-app-bar>
 
</template>
<script>
export default {
  data() {
    return {
      drawer: null,
    };
  },
};
</script>