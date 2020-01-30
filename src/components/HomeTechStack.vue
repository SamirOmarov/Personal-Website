<template >
  <div id="techstack">
    <v-container>
      <v-row no-gutters>

        <v-row justify="center">

          <v-col cols="12" lg="8" md="12" sm="10">
            <p class="my-5 text-important">WEB TECH STACK</p>
            <p class="mt-3 text-details">
              Single page Web app written in Vue and backend operations through RESTfull API powered by Python and Flask.
              Projects component uses Github REST API v3.
            </p>
          </v-col>
        </v-row>

        <v-row justify="center">
          <v-col cols="12" lg="2" md="3" sm="10" >
            <p class="text-details mt-5">Front End</p>
            <div class="subheading mt-3 text-description">
              <ul style="margin-top:10px;">
                <li>Vue.js</li>
                <li>Vuetify</li>
                <li>VantaJS</li>
              </ul>
            </div>
          </v-col>

          <v-col cols="12" lg="2" md="3" sm="10" >
            <p class="text-details mt-5">Back End</p>
            <div class="subheading mt-3 text-description">
              <ul style="margin-top:10px;">
                <li>Python</li>
                <li>Flask</li>
              </ul>
            </div>
          </v-col>

          <v-col cols="12" lg="2" md="3" sm="10" >
            <p class="text-details mt-5">Database</p>
            <div class="subheading mt-3 text-description">
              <ul style="margin-top:10px;">
                <li>PostgreSQL</li>
              </ul>
            </div>
          </v-col>

          <v-col cols="12" lg="2" md="3" sm="10" >
            <p class="text-details mt-5">Deployment</p>
            <div class="subheading mt-3 text-description">
              <ul style="margin-top:10px;">
                <li>Nginx</li>
                <li>Docker,Kubernetes</li>
                <li>AWS</li>
              </ul>
            </div>
          </v-col>
        </v-row>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  name: "HomeTechStack"
};
</script>

<style scoped>
#techstack {
  /* width: 100%; */
  background-color: #051622;
}
</style>