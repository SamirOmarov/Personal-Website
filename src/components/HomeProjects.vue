<template >
  <div id="projects">
    <v-container>
      <v-row no-gutters justify="center">
        <v-col cols="12" lg="8" md="12" sm="10" class="my-5">
          <p class="text-important">PROJECTS REPOSITORY</p>
          <v-data-table
            dark
            :headers="headers"
            :items="repos"
            :items-per-page="numberPerpage"
            class="elevation-1"
          >
            <template v-slot:item.name="{ item }">
              <a :href="item.html_url" target="_blank" class="custom-link">{{ item.name }}</a>
            </template>
          </v-data-table>
        </v-col>
      </v-row>
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

</style>