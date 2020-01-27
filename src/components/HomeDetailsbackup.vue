<template >
  <div id="about">
    <v-container>
      <v-layout column>
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
          <div class="headline mt-3 text-style">Lorem ipsum</div>
          <p
            class="subheading mt-3 text-style"
          >Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras pulvinar risus quis mauris interdum, in euismod nibh pretium. Etiam pulvinar tincidunt dapibus. Quisque sollicitudin, mauris a consequat consectetur, turpis nisl sollicitudin enim, id consectetur neque neque nec metus. Pellentesque dolor nisi, vulputate quis lobortis ac, tincidunt et quam. Mauris pulvinar blandit nisi nec mattis. Aliquam accumsan ut sem eget efficitur. Vivamus in tortor gravida eros laoreet condimentum nec vel dui. Nullam quam massa, ultrices eget tincidunt a, pulvinar ac libero.</p>

          <p
            class="subheading mt-3 text-style"
          >Nullam nec massa eu est fringilla lobortis. Praesent in enim in justo blandit varius. Cras placerat arcu in sapien rhoncus aliquet. Sed interdum tortor et tincidunt condimentum. Etiam consequat mi leo, in suscipit odio scelerisque molestie. Nam et purus consequat, iaculis augue vel, sagittis ligula. Vestibulum aliquet vulputate erat. Phasellus id mauris mauris. Nunc a maximus dolor. Curabitur ut vestibulum arcu. Curabitur non lacus justo. Cras varius a magna in semper. Nulla eros ante, consectetur faucibus sapien eu, rhoncus imperdiet dui. Sed viverra iaculis nunc, id pulvinar massa egestas vitae.</p>

          <p
            class="subheading mt-3 text-style"
          >Aenean erat metus, imperdiet eget nisl laoreet, venenatis ultricies ante. In interdum ante vel dictum ullamcorper. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Integer sit amet gravida diam. Aliquam in tempor metus. Fusce pellentesque pharetra sem, et luctus justo tempor dictum. Ut feugiat est sed tristique egestas. Nullam posuere a nunc in blandit. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Suspendisse laoreet ultrices eros, nec malesuada enim semper sit amet. Maecenas efficitur consectetur accumsan. Etiam in aliquam turpis, ut pharetra nulla. Vestibulum malesuada, nulla id elementum cursus, nibh dui rhoncus felis, suscipit mattis felis enim sed ex. Pellentesque scelerisque aliquam lorem, vel mattis nibh tincidunt ac. Suspendisse ac nibh sit amet lacus ullamcorper maximus.</p>
        </v-col>
        <v-col>
          <div class="headline mt-3 text-style">Lorem ipsum</div>
          <p
            class="subheading mt-3 text-style"
          >Nullam nec massa eu est fringilla lobortis. Praesent in enim in justo blandit varius. Cras placerat arcu in sapien rhoncus aliquet. Sed interdum tortor et tincidunt condimentum. Etiam consequat mi leo, in suscipit odio scelerisque molestie. Nam et purus consequat, iaculis augue vel, sagittis ligula. Vestibulum aliquet vulputate erat. Phasellus id mauris mauris. Nunc a maximus dolor. Curabitur ut vestibulum arcu. Curabitur non lacus justo. Cras varius a magna in semper. Nulla eros ante, consectetur faucibus sapien eu, rhoncus imperdiet dui. Sed viverra iaculis nunc, id pulvinar massa egestas vitae.</p>
        </v-col>
      </v-layout>
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