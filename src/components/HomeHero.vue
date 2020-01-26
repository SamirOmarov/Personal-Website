<template>
  <v-container fluid fill-height id="home-bg" style="max-height:100vh;">
    <v-layout justify-center align-center column pa-5>
      <div class="text-hero">SAMIR OMAROV</div>
      <div class="text-intro">Software and mechatronics engineering through research & development.</div>
      <v-btn text class="mt-10">
        <v-icon color="#1ba098" >Read More</v-icon>
      </v-btn>
    </v-layout>
  </v-container>
</template>


<script>
export default {
  mounted() {
    window.VANTA.WAVES({
      el: "#home-bg",
      mouseControls: true,
      touchControls: true,
      minHeight: 100.0,
      minWidth: 100.0,
      scale: 1.0,
      scaleMobile: 1.0,
      // color: 0x2f4350,
      color: 0x051622,
      shininess: 42.0,
      waveHeight: 15.5,
      zoom: 0.97
    });
  }
};
</script>



<style scoped>
@import url("https://fonts.googleapis.com/css?family=Montserrat|Raleway&display=swap");

.text-hero {
  font-family: "Gravity";
  color: #deb992;
  /* color: white; */
  letter-spacing: 20px;
  font-size: 40px;
  /* margin-inline-start: 10%;
  margin-inline-end: 10%; */
}

.text-intro {
  font-family: "Gravity";
  color: #deb992;
  /* color: white; */
  /* letter-spacing: 1vh; */
  font-size: 32px;
  /* display: block; */
  margin-block-start: 2em;
  margin-block-end: 2em;
  margin-inline-start: 10%;
  margin-inline-end: 10%;
}
</style>

