<template>
  <div id="footer">
    <footer class="footer">
      <p>
        ©2021 - Vaca e Cumadi Memator. Webapp criador de Memes
        <br />
        Criado por <a href="https://jcgsr.github.io/">Jovane</a>
        <br />
        <span id="rights">Todos os Direitos Reservados</span>
      </p>
    </footer>
  </div>
</template>
<script>
export default {
  name: "Footer",
};
</script>

<style lang="css">
.footer p {
  background-color: #101010;
  color: greenyellow;
  padding: 1rem;
  text-align: center;
}
#footer {
  font-size: smaller;
  width: 100%;
  box-shadow: 1px 1px 3px greenyellow;
  position: fixed;
  bottom: 0px;
  left: 0px;
  right: 0px;
  height: 80px;
}
p a {
  font-size: x-small;
  color: gray;
}
#rights {
  font-size: x-small;
  padding-top: 1rem;
}
</style>