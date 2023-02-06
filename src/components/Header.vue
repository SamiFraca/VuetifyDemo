<template>
  <v-app-bar app color="primary" dark class="mb-5">
    <div class="d-flex align-center">
      <span class="text-xl-h5">WatchMe</span>
    </div>
    <div class="w-50 ml-6 mt-3">
      <v-autocomplete style></v-autocomplete>
    </div>
    <v-spacer></v-spacer>
    <v-avatar color="red" size="45" class="mr-5">
      <img src="../assets/page.jpg" />
    </v-avatar>
    <div class="text-center">
      <v-menu offset-y transition="scroll-y-transition">
        <template v-slot:activator="{ on, attrs }">
          <v-btn color="red darken-2" dark v-bind="attrs" v-on="on">Dropdown</v-btn>
        </template>
        <v-list>
          <v-list-item v-for="(item, index) in items" :key="index">
            <v-list-item-title>{{ item.title }}</v-list-item-title>
          </v-list-item>
        </v-list>
      </v-menu>
    </div>
  </v-app-bar>
</template>

<script>
export default {
  data: () => ({
    items: [
      { title: "Click Me" },
      { title: "Click Me" },
      { title: "Click Me" },
      { title: "Click Me 2" },
    ],
  }),
  methods: {
    Dropdown() {
      for (let i = 0; i < this.items.length; i++) {
        let openDropdown = this.items[i];
        if (openDropdown.classList.contains("show")) {
          openDropdown.classList.remove("show");
        }
      }
    },
  },
};
</script>

<style>
</style>