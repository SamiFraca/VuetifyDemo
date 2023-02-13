<template>
  <v-app>
    <v-main>
      <Header />
      <Calendar />
      <div style="display:flex;">
        <Card />
        <Card />
        <Card />
      </div>
      <Carousel />
      <MobileNavBottom />
      <Footer />
    </v-main>
  </v-app>
</template>

<script>
import {
  Calendar,
  Header,
  Footer,
  MobileNavBottom,
  Card,
  Carousel,
  HeaderText,
  HeaderTextWrapper,
} from "./components/index";
export default {
  name: "App",

  components: {
    Calendar,
    Header,
    Footer,
    MobileNavBottom,
    Card,
    Carousel,
  },

  data: () => ({
    items: [
      { title: "Test" },
      { title: "Test" },
      { title: "Test" },
      { title: "Click Me 2" },
    ],
    model: 0,
    colors: ["primary", "secondary", "yellow darken-2", "red", "orange"],
  }),
};
</script>
<style>
@import url("https://fonts.googleapis.com/css2?family=Merienda&display=swap");
</style>