<template >
  <div id="projects">
    <v-container>
      <v-col class="text-xs-center my-5 text-important">GITHUB PROJECTS</v-col>

      <v-data-table
        dark
        :headers="headers"
        :items="repos"
        :items-per-page="numberPerpage"
        class="elevation-1"
      >
        <template v-slot:item.name="{ item }">
          <a :href="item.html_url" class="custom-link">{{ item.name }}</a>
        </template>
      </v-data-table>
    </v-container>
  </div>
</template>


<script>
import axios from "axios";

export default {
  name: "HomeProjects",

  data: function() {
    return {
      headers: [
        { text: "Title", align: "left", value: "name" },
        { text: "Description", value: "description" },
        { text: "Language", value: "language" },
        { text: "Stars", value: "stargazers_count" }
        // { text: "", value: "html_url" }
      ],
      numberPerpage: 5,
      repos: []
    };
  },

  mounted: function() {
    this.getRepos();
  },

  methods: {
    getRepos: function() {
      let self = this;
      axios
        .get(`https://api.github.com/users/SamirOmarov/repos`, {
          params: {
            sort: "updated"
          }
        })
        .then(response => {
          self.repos = response.data;
        })
        .catch(error => {
          console.log(error);
        });
    }
  }
};
</script>

<style scoped>
.custom-link {
  color: white;
  text-decoration: unset;
  font-weight: 700;
}
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