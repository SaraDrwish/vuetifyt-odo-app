<template>
  <v-app id="inspire">
    <v-navigation-drawer v-model="drawer" app>
      <!--  -->
      <!-- <v-list>
        <v-list-item>
          <span>kladlkann</span>
        </v-list-item>
      </v-list> -->
      <v-list-item>
        <v-list-item-content>
          <v-list-item-title>
            <span>title</span>
          </v-list-item-title>
          <v-list-item-subtitle>
            <span>subtitle</span>
          </v-list-item-subtitle>
        </v-list-item-content>
      </v-list-item>

      <v-divider></v-divider>
      <v-list density="compact" nav>
        <v-list-item>
          <v-btn text>
            <v-icon>mdi-account</v-icon>
          </v-btn>
          <span>shared </span>
        </v-list-item>

        <v-list-item>
          <v-btn text>
            <v-icon>mdi-account-multiple</v-icon>
          </v-btn>
          <span>shared with me </span>
        </v-list-item>

        <v-list-item prepend-icon="mdi-star" title="Starred" value="starred">
          <v-btn text>
            <v-icon>mdi-folder</v-icon>
          </v-btn>
          <span>My Files</span>
        </v-list-item>
      </v-list>
      <!-- <span>sdfdsfsd</span> -->
    </v-navigation-drawer>

    <v-app-bar app>
      <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>

      <v-toolbar-title>Sara's Todo Application</v-toolbar-title>
    </v-app-bar>

    <v-main>
      <!--  -->
      <span class="pa-8 red yellow--text"> helooo </span>
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
