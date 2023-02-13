<template>
  <v-carousel v-model="model">
    <v-carousel-item v-for="(color) in colors" :key="color">
      <v-sheet :color="color" height="100%" tile>
        <v-row class="fill-height" align="center" justify="center">
          <div class="text-h2">WATCHME</div>
        </v-row>
      </v-sheet>
    </v-carousel-item>
  </v-carousel>
</template>

<script>
export default {
  data: () => ({
    model: 0,
    colors: ["green", "secondary", "yellow darken-2", "red", "orange"],
  }),
};
</script>

<style>
</style>