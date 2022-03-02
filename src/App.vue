<template>
  <div id="app">
    <Header />
    <router-view />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/header/header";
import Footer from "./components/footer/footer";

export default {
  name: "HelloWorld",
  props: {},
  components: {
    Header,
    Footer,
  },
};
</script>

<style lang="scss">
@import "./css/styles";
</style>
