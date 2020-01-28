<template >
  <div id="projects">
    <v-container>
      {{ getRepos() }}
      <v-row no-gutters>
        <v-row>
          <v-col class="text-xs-center my-5 text-important">FAVOURITE PROJECTS</v-col>
        </v-row>
        <v-row>
          <v-col>
            <div v-for="repo in repos" v-bind:key="repo">
                <!-- For table need .name (inside .html_url)
                .description .language .stargazers_count-->
              <p class="text-important">{{ repo.name }}</p>
              <p class="text-description">{{ repo.description }}</p>
            </div>
          </v-col>
        </v-row>
      </v-row>
    </v-container>
  </div>
</template>


<script>
import axios from "axios";

export default {
  name: "HomePlans",

  data: function() {
    return {
      repos: null
    };
  },

  methods: {
    getRepos: function() {
      return axios
        .get(`https://api.github.com/users/SamirOmarov/repos`)
        .then(response => {
          this.repos = response.data;
        })
        .catch(error => {
          console.log(error);
        });
    }

    // async getNumberofFollowers() {
    //   let res = await axios.get("https://api.github.com/users/SamirOmarov");
    //     let followers = res.data.followers;
    //     let location = res.data.location;

    // }
  }
};
</script>

<style scoped>
#projects {
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
  margin-inline-start: 12%;
  margin-inline-end: 10%;
}

.text-style {
  font-family: "Gravity";
  color: #deb992;
  /* color: white; */
  letter-spacing: 10px;
  font-size: 30px;
  margin-block-start: 2em;
  margin-block-end: 2em;
  margin-inline-start: 12%;
  margin-inline-end: 10%;
}

.text-description {
  font-family: "Gravity";
  color: white;
  letter-spacing: 10px;
  font-size: 16px;
  /* margin-block-start: 2em; */
  /* margin-block-end: 2em; */
  margin-inline-start: 12%;
  margin-inline-end: 10%;
}
</style>