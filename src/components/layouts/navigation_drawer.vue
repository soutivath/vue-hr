<template>
 
    <v-navigation-drawer
      v-if="$vuetify.breakpoint.mdAndUp"
      permanent
      floating
      app
      color="#202040"
      dark
      style="background: radial-gradient(circle, rgba(0,0,0,0.4489146000196954) 6%, rgba(0,0,0,0.8578781854538691) 76%);"
      :mini-variant="displayMini"
      mini-variant-width="80"
      :expand-on-hover="displayMini?true:false"
    >
      <v-list-item>
        <v-list-item-content>
          <v-list-item-title>
            <v-img src=""></v-img>
          </v-list-item-title>
          <v-list-item-subtitle class="ml-10" v-if="displayMini==false">Kasumi best girl</v-list-item-subtitle>
        </v-list-item-content>
      </v-list-item>
      <v-divider></v-divider>

      <v-list dense nav>
        <v-list-item link>
          <v-list-item-icon>
            <v-icon>mdi mdi-abugida-devanagari</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title>ພະນັກງານ</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
      <v-list dense nav>
        <v-list-item link>
          <v-list-item-icon>
            <v-icon>mdi mdi-abugida-devanagari</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title>ສາຂາ</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
      <v-list dense nav>
        <v-list-item link>
          <v-list-item-icon>
            <v-icon>mdi mdi-abugida-devanagari</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title>ພະແນກ</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-navigation-drawer
      v-else
      right
      v-model="drawer"
      floating
      app
      color="#202040"
      dark
      style="background: radial-gradient(circle, rgba(0,0,0,0.4489146000196954) 6%, rgba(0,0,0,0.8578781854538691) 76%);"
    >
      <v-list-item>
        <v-list-item-content>
          <v-list-item-title>Application</v-list-item-title>
          <v-list-item-subtitle>Subtext</v-list-item-subtitle>
        </v-list-item-content>
      </v-list-item>
      <v-divider></v-divider>

      <v-list dense nav>
        <v-list-item link>
          <v-list-item-icon>
            <v-icon>mdi mdi-abugida-devanagari</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title>Employee</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
      <v-list dense nav>
        <v-list-item link>
          <v-list-item-icon>
            <v-icon>mdi mdi-abugida-devanagari</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title>Employee</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
      <v-list dense nav>
        <v-list-item link>
          <v-list-item-icon>
            <v-icon>mdi mdi-abugida-devanagari</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title>Employee</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
  
</template>
<script>
export default {
  data() {
    return {
      
      displayMini: false,
    };
  },
};
</script>