<template>
  <div id="app">
    <AppHeader></AppHeader>
    <ContentArea></ContentArea>
    <AppFooter></AppFooter>
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader";
import AppFooter from "./components/AppFooter";
import ContentArea from "./components/ContentArea";

export default {
  name: 'app',
  components: {
    AppHeader,
    AppFooter,
    ContentArea
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
