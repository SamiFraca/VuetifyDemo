<template>
  <v-bottom-navigation
    :value="value"
    color="primary"
    background-color="whitesmoke"
    class="d-lg-none d-md-none"
    grow
  >
  <Badge/>
    <v-btn>
      <span>Recents</span>

      <v-icon>mdi-history</v-icon>
    </v-btn>

    <v-btn>
      <span>Favorites</span>

      <v-icon>mdi-heart</v-icon>
    </v-btn>

    <v-btn>
      <span>Nearby</span>

      <v-icon>mdi-map-marker</v-icon>
    </v-btn>
  </v-bottom-navigation>
</template>

<script>
import Badge from './Badge'
export default {
  components: Badge,
  data: () => ({ value: 1 }),
};
</script>

<style>
</style>