<template>
  <v-container fluid fill-height id="home-bg" style="max-height:100vh;">
    <v-row justify="center" no-gutters>
      <v-col cols="12" lg="8" md="9" sm="10" class="my-5" >
        <p class="text-hero text-center">SAMIR OMAROV</p>
        <p class="text-intro text-center ">
          Software and mechatronics engineering through
          research & development.
        </p>

        <div class="text-center">
        <v-btn text style="margin-top:10%">
          <v-icon v-scroll-to="{ el: '#about', offset: -50 }" color="#1ba098">READ MORE</v-icon>
        </v-btn>
        </div>
      </v-col>
    </v-row>
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
  letter-spacing: 20px;
  font-size: 40px;
}

.text-intro {
  font-family: "Gravity";
  color: #deb992;
  font-size: 32px;
}
</style>

