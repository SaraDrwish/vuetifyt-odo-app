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
            <h3>Vuetify Todo</h3>
          </v-list-item-title>
          <v-list-item-subtitle>
            <span>best todo ever !</span>
          </v-list-item-subtitle>
        </v-list-item-content>
      </v-list-item>

      <v-divider></v-divider>

      <v-list density="compact" nav>
        <!-- ///// -->
        <!-- <v-list-item link>
          <v-icon>mdi-view-dashboard</v-icon>
          <span>Todo </span>
        </v-list-item>

        <v-list-item link>
          <v-btn text>
            <v-icon>mdi-account-multiple</v-icon>
          </v-btn>
          <span>About</span>
        </v-list-item> -->
        <!-- ///////// -->
        <v-list-item v-for="it in items" :key="it" link>
          <v-list-item-icon>
            <v-icon> {{ it.icon }}</v-icon>
          </v-list-item-icon>
          <v-list-item-content>{{ it.title }}</v-list-item-content>
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
      <span class="pa-8 red yellow--text"> Helooo </span>
    </v-main>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      drawer: null,
      items: [
        { id: 1, title: "Dashboard", icon: "mdi-view-dashboard" },
        { id: 2, title: "About", icon: "mdi-account" },
        { id: 3, title: "Star", icon: "mdi-star" },
      ],
    };
  },
};
</script>
