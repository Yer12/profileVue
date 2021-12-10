<template>
  <Container />
</template>

<script>
import Container from "./components/Container";

export default {
  name: 'App',
  components: {
    Container,

  }
}
</script>

<style>
html,body {
  margin: 0;
  padding: 0;
  background: rgba(203, 194, 153, 0.3);
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;

}
.d-flex {
  display: flex;
}
</style>
