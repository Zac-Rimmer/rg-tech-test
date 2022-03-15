<template>
  <header class="d-flex justify-content-between">
    <img src="../../assets/images/Regatta-Group-Logo.png" alt="Regatta Group" id="logo" />
    <Navigation />
  </header>
</template>

<script>

import Navigation from "@/components/navigation/navigation.vue";
export default {
  name: "Header",
  props: {},
  components:{
    Navigation,
  }
};
</script>

<style scoped lang="scss">
#logo {
  max-width: 200px;
}
</style>
