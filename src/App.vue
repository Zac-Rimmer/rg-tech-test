<template>
  <div id="app">
    <Header />
    <USP />
    <router-view />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/header/header";
import Footer from "./components/footer/footer";
import USP from "./components/header/usp";

export default {
  name: "HelloWorld",
  props: {},
  components: {
    Header,
    Footer,
    USP,
  },
};
</script>

<style lang="scss">
@import "./css/styles";
</style>
