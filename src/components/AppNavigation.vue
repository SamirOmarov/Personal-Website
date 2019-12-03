<template>
  <span>
    <v-navigation-drawer app v-model="drawer" class dark disable-resize-watcher>
      <v-list>
        <template v-for="(item, index) in items">
          <v-list-tile :key="index">
            <v-list-tile-content>{{item.title}}</v-list-tile-content>
          </v-list-tile>
          <v-divider :key="`divider-${index}`"></v-divider>
        </template>
      </v-list>
    </v-navigation-drawer>

    <v-toolbar app color="blue-grey darken-4" dark>
      <v-toolbar-side-icon class="hidden-md-and-up" @click="drawer = !drawer"></v-toolbar-side-icon>
      <v-spacer class="hidden-md-and-up"></v-spacer>
      <v-toolbar-title>{{ appTitle }}</v-toolbar-title>
      <v-btn text class="hidden-sm-and-down">About</v-btn>
      <v-btn text class="hidden-sm-and-down">Projects</v-btn>
      <v-spacer class="hidden-sm-and-down"></v-spacer>
      <v-btn text class="hidden-sm-and-down">Contact</v-btn>
    </v-toolbar>
  </span>
</template>

<script>
export default {
  name: "AppNavigation",
  data() {
    return {
      appTitle: "Samir Omarov",
      drawer: false,
      items: [{ title: "About" }, { title: "Projects" }, { title: "Contact" }]
    };
  }
};
</script>

<style scoped>
</style>
