<template>
  <v-app>
    <Navbars class="fontnav"></Navbars>
    <v-content>
      <v-container>
        <v-row>
          <v-col md="12">
            <tableComponent class="fontnew"></tableComponent>
          </v-col>
        </v-row>
      </v-container>
    </v-content>
  </v-app>
</template>
<script>
import Navbars from "@/components/DashboardLayout/navbars";
import tableComponent from "./components/table.vue";
export default {
  components: {
    tableComponent,
    Navbars,
  },
};
</script>
<style>
@font-face {
  font-family: fontlao;
  src: url("./assets/font/boonhome-700.woff");
}
.fontnav,
.fontnew {
  font-family: fontlao;
}
</style>
