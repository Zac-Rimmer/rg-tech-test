<template>
  <div id="app">
    <Header />
    <router-view />
  </div>
</template>

<script>
import Header from "./components/header/header";

export default {
  name: "HelloWorld",
  props: {},
  components: {
    Header,
  },
};
</script>

<style lang="scss">
@import "./css/styles";
</style>
