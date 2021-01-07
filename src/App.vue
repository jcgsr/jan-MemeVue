<template>
  <div id="app">
    <Header />
    <MemeGenerator />
    <Footer />
  </div>
</template>

<script>
import MemeGenerator from "./components/MemeGenerator.vue";
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "app",
  components: {
    MemeGenerator,
    Header,
    Footer,
  },
};
</script>

<style lang="css">
@import url("https://fonts.googleapis.com/css2?family=Goldman&display=swap");
body {
  background-color: rgb(25, 59, 22);
  font-family: "Goldman", cursive;
  margin-bottom: 100px;
}
</style>
