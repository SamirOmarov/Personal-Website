<template>
  <span>
    <v-navigation-drawer app v-model="drawer" class light disable-resize-watcher>
      <v-list>
        <template v-for="(item, index) in items">
          <v-list-item :key="index">
            <v-list-item-content>{{item.title}}</v-list-item-content>
          </v-list-item>
          <v-divider :key="`divider-${index}`"></v-divider>
        </template>
      </v-list>
    </v-navigation-drawer>

    <v-app-bar app fixed color="" light>
      <v-app-bar-nav-icon class="hidden-md-and-up" @click="drawer = !drawer"></v-app-bar-nav-icon>
      <v-spacer class="hidden-md-and-up"></v-spacer>
      <v-toolbar-title>{{ appTitle }}</v-toolbar-title>
      <v-btn text class="hidden-sm-and-down">About</v-btn>
      <v-btn text class="hidden-sm-and-down">Projects</v-btn>
      <v-spacer class="hidden-sm-and-down"></v-spacer>
      <v-btn text class="hidden-sm-and-down">Contact</v-btn>
    </v-app-bar>
  </span>
</template>

<script>
export default {
  name: "AppNavigation",
  data() {
    return {
      appTitle: "Samir Omarov",
      drawer: false,
      dropdown_items: ["About", "Projects", "Contact"],
      items: [{ title: "About" }, { title: "Projects" }, { title: "Contact" }]
    };
  }
};
</script>

<style scoped>
</style>
