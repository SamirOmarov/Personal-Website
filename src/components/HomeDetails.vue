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
          <div class="subheading mt-3 text-skills">
            Here are a few technologies I've been working with recently:
            <ul style="margin-top:10px;">
              <li>Python: Django, Flask, Automation</li>
              <li>C/C++: Low level/embedded IoT programming</li>
              <li>Vue.js: Vuetify</li>
              <li>Flutter</li>
              <li>PostgreSQL</li>
              <li>Docker,Kubernetes</li>
              <li>HTML & (S)CSS</li>
            </ul>
          </div>
        </v-col>
        <v-col>
          <div class="mt-3 text-heading">Data Science & ML</div>
          <div class="subheading mt-3 text-skills">
            I love training deep learning models on large datasets
            <ul style="margin-top:10px;">
              <li>Python essentials</li>
              <li>Pytorch, Tensorflow</li>
              <li>Data Modeling & Evaluation</li>
              <li>Distributed Computing: AWS, Kaggle</li>
              <li>Windows & Linux</li>
              <li>Git</li>
              <li>Web Scraping</li>
            </ul>
          </div>
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
li {
  /* list-style-type: none; */
  margin-top: 8px;
}

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
  font-size: 24px;

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
  font-size: 18px;
  /* display: block; */
  margin-block-start: 2em;
  margin-block-end: 2em;
  margin-inline-start: 20%;
  margin-inline-end: 20%;
}

.text-style {
  font-family: "Gravity";
  /* color: #deb992; */
  color: white;
  /* letter-spacing: 1vh; */
  font-size: 22px;
  /* display: block; */
  margin-block-start: 2em;
  margin-block-end: 2em;
  margin-inline-start: 10%;
  margin-inline-end: 10%;
}
</style>