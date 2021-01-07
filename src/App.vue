<template>
  <div id="app">
    <Header />
    <MemeGenerator />
    <p>{{ currentDate }}</p>
    <Footer />
  </div>
</template>

<script>
import MemeGenerator from "./components/MemeGenerator.vue";
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "app",
  data: () => ({
    currentDate: "Data de hoje...",
  }),
  components: {
    MemeGenerator,
    Header,
    Footer,
  },
  methods: {
    dataAtual: function () {
      let hoje = new Date();
      this.currentDate = hoje.toLocaleDateString("pt-BR", {
        day: "2-digit",
        month: "short",
        year: "numeric",
      });
    },
  },
  mounted() {
    this.dataAtual()
  }
};
</script>

<style lang="css">
@import url("https://fonts.googleapis.com/css2?family=Goldman&display=swap");
body {
  background-color: rgb(25, 59, 22);
  font-family: "Goldman", cursive;
  margin-bottom: 100px;
  color: yellow;
}
p {
  text-align: center;
  padding: 2rem;
  margin: 0;
  font-size: small;
}
</style>
