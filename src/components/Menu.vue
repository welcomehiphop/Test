<template>
  <v-navigation-drawer permanent absolute xs class="mt-16">
    <v-list-item>
      <v-list-item-content>
        <v-list-item-title class="title">
          Menu
        </v-list-item-title>
        <!-- <v-list-item-subtitle>
            subtext
          </v-list-item-subtitle> -->
      </v-list-item-content>
    </v-list-item>
    <v-divider dark></v-divider>
    <v-list dense nav>
      <v-list-item-group v-model="selectedItem" color="primary">
        <v-list-item
          v-for="item in items"
          :key="item.title"
          @click="onClickMenu(item.route)"
        >
          <v-list-item-icon>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title>{{ item.title }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list-item-group>
    </v-list>
  </v-navigation-drawer>
</template>

<script>
export default {
  data() {
    return {
      selectedItem: "",
      items: [
        { title: "Menu1", icon: "mdi-home", route: "/home" },
        { title: "Menu2", icon: "mdi-file-document-outline", route: "/about" },
        { title: "Menu3", icon: "mdi-file-document-outline", route: "/about" },
        { title: "Menu4", icon: "mdi-file-document-outline", route: "/about" },
      ],
      right: null,
    };
  },
  methods: {
    onClickMenu(menu) {
      console.log(menu);
      this.$router.push(menu);
    },
  },
};
</script>

<style scoped>
.v-list-item-title {
  background: black;
}
.title {
  background: primary;
  font-size: 24px !important;
  /* background: black; */
}
</style>
