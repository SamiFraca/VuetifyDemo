<template>
  <v-card class="mx-auto my-8" max-width="400" tile>
    <v-list-item>
      <v-list-item-content>
        <v-list-item-title>
          <span class="pa-2">
            <Badge />
          </span>
          Single-line item
        </v-list-item-title>
      </v-list-item-content>
    </v-list-item>

    <v-list-item two-line>
      <v-list-item-content>
        <v-list-item-title>Two-line item</v-list-item-title>
        <v-list-item-subtitle>Secondary text</v-list-item-subtitle>
      </v-list-item-content>
    </v-list-item>

    <v-list-item three-line>
      <v-list-item-content>
        <v-list-item-title>Three-line item</v-list-item-title>
        <v-list-item-subtitle>Secondary line text Lorem ipsum dolor sit amet,</v-list-item-subtitle>
        <v-list-item-subtitle>consectetur adipiscing elit.</v-list-item-subtitle>
      </v-list-item-content>
    </v-list-item>
  </v-card>
</template>
<script>
import Badge from "./Badge";
export default {
  name: "Card",
  components: { Badge: Badge },
};
</script>

<style>
</style>