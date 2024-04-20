<template>
  <v-app id="inspire">
    <v-navigation-drawer v-model="drawer" app>
      <!--  -->
      <v-list>
        <v-list-item
          prepend-avatar="https://randomuser.me/api/portraits/women/85.jpg"
          subtitle="sandra_a88@gmailcom"
          title="Sandra Adams"
        ></v-list-item>
      </v-list>

      <v-divider></v-divider>

      <v-list density="compact" nav>
        <v-list-item prepend-icon="mdi-folder" title="My Files" value="myfiles">
          <v-btn text>
            <v-icon>mdi-folder</v-icon>
          </v-btn>
          <span>My Files</span>
        </v-list-item>
        <v-list-item
          prepend-icon="mdi-account-multiple"
          title="Shared with me"
          value="shared"
        >
          <v-btn text>
            <v-icon>mdi-account-multiple</v-icon>
          </v-btn>
          <span>shared with me </span>
        </v-list-item>

        <v-list-item prepend-icon="mdi-star" title="Starred" value="starred">
          <v-btn text>
            <v-icon>mdi-star</v-icon>
          </v-btn>
          <span>Starred </span>
        </v-list-item>
      </v-list>
      <!-- <span>sdfdsfsd</span> -->
    </v-navigation-drawer>

    <v-app-bar app>
      <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>

      <v-toolbar-title>Application</v-toolbar-title>
    </v-app-bar>

    <v-main>
      <!--  -->
      <span> kllllllee </span>
    </v-main>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      drawer: null,
    };
  },
};
</script>
