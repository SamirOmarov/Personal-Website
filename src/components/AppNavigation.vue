<template>
  <span>
    <v-navigation-drawer app v-model="drawer" color="#051622" disable-resize-watcher>
      <v-list>
        <template v-for="(item, index) in items">
          <v-list-item :key="index">
            <v-list-item-group
              v-scroll-to="{el:'#'+item.id, offset: -50}"
              color="#1ba098"
            >{{item.title}}</v-list-item-group>
          </v-list-item>
          <v-divider :key="`divider-${index}`"></v-divider>
        </template>
      </v-list>
    </v-navigation-drawer>

    <v-app-bar app dense color="#051622">
      <v-app-bar-nav-icon color="#1ba098" class="hidden-md-and-up" @click="drawer = !drawer"></v-app-bar-nav-icon>
      <v-spacer class="hidden-md-and-up"></v-spacer>
      <v-btn text color="#1ba098" v-scroll-to="'#home-bg'">{{ appTitle }}</v-btn>
      <v-spacer class="hidden-sm-and-down"></v-spacer>
      <v-btn
        v-scroll-to="{ el: '#about', offset: -50 }"
        text
        class="hidden-sm-and-down"
        color="#1ba098"
      >About</v-btn>
      <v-btn
        v-scroll-to="{ el: '#projects', offset: -50 }"
        text
        class="hidden-sm-and-down"
        color="#1ba098"
      >Projects</v-btn>
      <v-btn
        v-scroll-to="{ el: '#techstack', offset: -50 }"
        text
        class="hidden-sm-and-down"
        color="#1ba098"
      >Tech Stack</v-btn>
      <v-btn
        v-scroll-to="{ el: '#contact', offset: -50 }"
        text
        class="hidden-sm-and-down"
        color="#1ba098"
      >Contact</v-btn>
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
      // dropdown_items: ["About", "Projects", "Contact"],
      items: [
        { title: "Home", id: "home-bg" },
        { title: "About", id: "about" },
        { title: "Projects", id: "projects" },
        { title: "Tech Stack", id: "techstack" },
        { title: "Contact", id: "contact" }
      ]
    };
  }
};
</script>

<style scoped>
.text-green {
  color: #1ba098;
}
</style>
