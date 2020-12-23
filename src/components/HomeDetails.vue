<template >
  <div id="about">
    <v-container>
      <v-row no-gutters>
        
        <v-row justify="center">
          <v-col cols="12" lg="8" md="12" sm="10">
            <p class="my-5 text-important">MY WORK</p>
            <p class="mt-3 text-details">
              I always had a desire to know how things work, wanted to learn by experience & yearned to
              solve challenging problems. A desire to extend my knowledge and an enthusiasm to solve the
              demanding problems, motivated me to pursue Degree in Mechatronics Engineering.
            </p>
          </v-col>
        </v-row>

        <v-row justify="center">
          <v-col cols="12" lg="4" md="6" sm="10">
            <div class="mt-3 text-heading">Software Development</div>
            <div class="subheading mt-3 text-skills">
              Here are a few technologies I've been working with recently:
              <ul style="margin-top:10px;">
                <li>Python: Django, Flask, Automation</li>
                <li>C/C++: Low level/embedded IoT programming</li>
                <li>Rust</li>
                <li>HTML & (S)CSS</li>
                <li>Vue.js: Vuetify</li>
                <li>Flutter</li>
                <li>PostgreSQL, MongoDB</li>
                <li>Docker,Kubernetes</li>
                <li>Version Control: GIT </li>
              </ul>
            </div>
          </v-col>
          <v-col cols="12" lg="4" md="6" sm="10">
            <div class="mt-3 text-heading">Data Science & ML</div>
            <div class="subheading mt-3 text-skills">
              I love training deep learning models on large datasets
              <ul style="margin-top:10px;">
                <li>Python essentials</li>
                <li>Pytorch, Tensorflow</li>
                <li>Data Modeling & Evaluation</li>
                <li>Computer Vision, NLP</li>
                <li>Data Mining & Visualization</li>
                <li>Data & Quantitative Analysis</li>
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

</style>
