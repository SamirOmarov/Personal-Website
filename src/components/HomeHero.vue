<template>
  <v-container fluid fill-height class="home-hero" style="max-height:100vh;">
    <v-layout justify-center align-center column pa-5>
      <div class="text-hero">SAMIR OMAROV</div>
      <div
        class="text-intro"
      >Software and mechatronics engineering through research & development.</div>
      <v-btn text class="mt-5">
        <v-icon color="white">Read More</v-icon>
      </v-btn>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  name: "HomeHero"
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css?family=Montserrat|Raleway&display=swap");

.text-hero {
  font-family: "Gravity";
  color: white;
  letter-spacing: 10px;
  font-size: 40px;
}

.text-intro {
  font-family: "Gravity";
  color: white;
  /* letter-spacing: 1vh; */
  font-size: 28px;
  display: block;
  margin-block-start: 1em;
  margin-block-end: 1em;
  margin-inline-start: 0px;
  margin-inline-end: 0px;
  /* font-weight: bold; */
}

.home-hero {
  background: url("https://ktechgmbh.com/wp-content/uploads/2019/04/portfolio.jpg");
  background-size: cover;
  width: 100%;
  height: 100%;
}
</style>