<template>
  <v-card class="mx-auto overflow-hidden " height="90">
    <v-system-bar color="deep-purple darken-3"></v-system-bar>

    <v-app-bar color="deep-purple accent-4" prominent>
      <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>

      <v-spacer></v-spacer>

      <v-btn icon>
        <v-icon>mdi-magnify</v-icon>
      </v-btn>

      <v-btn icon>
        <v-icon>mdi-filter</v-icon>
      </v-btn>

      <v-btn icon>
        <v-icon>mdi-dots-vertical</v-icon>
      </v-btn>
    </v-app-bar>

    <v-navigation-drawer
      v-model="drawer"
      absolute
      bottom
      temporary
      height="500"
    >
      <v-list nav dense>
        <v-list-item-group
          v-model="group"
          active-class="deep-purple--text text--accent-4"
        >
          <v-list-item>
            <v-list-item-title>
              <button>
                <router-link
                  to="/"
                  style="text-decoration: none; color: inherit;"
                >
                  Home
                </router-link>
              </button>
            </v-list-item-title>
          </v-list-item>
          <v-list-item>
            <v-list-item-title>
              <button>
                <router-link
                  to="/about"
                  style="text-decoration: none; color: inherit;"
                >
                  About Us
                </router-link>
              </button>
            </v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-title>
              <button>
                <router-link
                  to="/Contact"
                  style="text-decoration: none; color: inherit;"
                >
                  Contact
                </router-link>
              </button>
            </v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-title>
              <button>
                <router-link
                  to="/Jbo"
                  style="text-decoration: none; color: inherit;"
                >
                  Job
                </router-link>
              </button>
            </v-list-item-title>
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>
  </v-card>
</template>
<script>
export default {
  data: () => ({
    drawer: false,
    group: null,
  }),

  watch: {
    group() {
      this.drawer = false;
    },
  },
};
</script>
<style scoped></style>
