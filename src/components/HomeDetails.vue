<template >
  <div id="about">
    <v-container>
      <v-row no-gutters>
        <v-row>
          <v-col class="text-xs-center my-5 text-important">MY WORK</v-col>
        </v-row>
        <v-row>
          <v-col>
            <p class="mt-3 text-style">
              I always had a desire to know how things work, wanted to learn by experience & yearned to
              solve challenging problems. A desire to extend my knowledge and an enthusiasm to solve the
              demanding problems, motivated me to pursue Degree in Mechatronics Engineering.
            </p>
          </v-col>
        </v-row>

        <v-col>
          <div class="mt-3 text-heading">Software Development</div>
          <p
            class="subheading mt-3 text-skills"
          >Lorem ipsum uris interdumcidunt dapibus. Quisque sollicitudin, mauris a consequat consectetur, turpis nisl sollicitudin enim, id consectetur neque neque nec metus. Pellentesque dolor nisi, vulputate quis lobortis ac, tincidunt et quam. Mauris pulvinar blandit nisi nec mattis. Aliquam accumsan ut sem eget efficitur. Vivamus in tortor gravida eros laoreet condimentum nec vel d</p>
        </v-col>
        <v-col>
          <div class="mt-3 text-heading">Data Science</div>
          <p
            class="subheading mt-3 text-skills"
          >Nullam nec r massa egestas vitae. dhaihiduwah adhiawhd haidhiuaqhd aiwdhiuaq</p>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  name: "HomeDetails"
};
</script>

<style scoped>
#about {
  width: 100%;
  background-color: #051622;
}

.text-important {
  font-family: "Gravity";
  color: #deb992;
  /* color: white; */
  letter-spacing: 10px;
  font-size: 30px;
  margin-block-start: 2em;
  margin-block-end: 2em;
  margin-inline-start: 10%;
  margin-inline-end: 10%;
}



.text-heading {
  font-family: "Gravity";
  color: #deb992;
  /* color: white; */
  letter-spacing: 10px;
  font-size: 26px;

  margin-block-start: 2em;
  margin-block-end: 2em;
  margin-inline-start: 20%;
  margin-inline-end: 20%;
}

.text-skills {
  font-family: "Gravity";
  /* color: #deb992; */
  color: white;
  /* letter-spacing: 1vh; */
  font-size: 24px;
  /* display: block; */
  margin-block-start: 2em;
  margin-block-end: 2em;
  margin-inline-start: 20%;
  margin-inline-end: 10%;
}

.text-style {
  font-family: "Gravity";
  /* color: #deb992; */
  color: white;
  /* letter-spacing: 1vh; */
  font-size: 24px;
  /* display: block; */
  margin-block-start: 2em;
  margin-block-end: 2em;
  margin-inline-start: 10%;
  margin-inline-end: 10%;
}



</style>