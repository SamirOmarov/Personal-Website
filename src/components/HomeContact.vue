<template >
  <div id="contact">
    <v-container>
      <v-row no-gutters justify="center">
        <v-col cols="12" lg="8" md="9" sm="10" class="my-10">
          <p class="text-center text-heading">STAY CONNECTED</p>
          <v-row justify="space-around" class="my-5">
            <a href="https://github.com/SamirOmarov" target="_blank">
              <v-icon large color="#1ba098">mdi-github-circle</v-icon>
            </a>
            <a href="https://www.linkedin.com/in/samiromarov/" target="_blank">
              <v-icon large color="#1ba098">mdi-linkedin</v-icon>
            </a>
            <a href="mailto:samir.omarov@gmail.com" target="_blank">
              <v-icon large color="#1ba098">mdi-gmail</v-icon>
            </a>
          </v-row>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  name: "HomeContact"
};
</script>

<style scoped>
#contact {
  background-color: #051622;
}
</style>