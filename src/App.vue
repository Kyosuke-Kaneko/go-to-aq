<template>
    <v-app>
        <v-navigation-drawer
                app
                v-model="drawer"
                clipped
        >Navigation Lists
        </v-navigation-drawer>
        <v-app-bar
                color="primary"
                dark
                :collapse="!collapseOnScroll"
                :collapse-on-scroll="collapseOnScroll"
                elevate-on-scroll
                app
                clipped-left>
            <v-app-bar-nav-icon @click="drawer=!drawer"></v-app-bar-nav-icon>
            <v-checkbox
                    v-model="collapseOnScroll"
                    color="white"
                    hide-details
            ></v-checkbox>
            <v-toolbar-title>Vuetify</v-toolbar-title>
        </v-app-bar>
        <v-footer color="primary" dark app>
            Vuetify
        </v-footer>
        <v-container style="height: 1500px;">
        </v-container>
    </v-app>
</template>

<script>
export default {
  data() {
    return {
      collapseOnScroll: true,
      // clipped: true,
      drawer: null
    }
  }
}
</script>