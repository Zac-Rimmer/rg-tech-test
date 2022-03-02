<template>
  <header class="d-flex justify-content-between align-items-center">
    <img src="../../assets/images/Regatta-Group-Logo.png" alt="Regatta Group" id="logo" />
	<Nav />
  </header>
</template>

<script>
import Nav from "@/components/header/nav.vue";

export default {
  name: "Header",
  components: {
	Nav,
  },
  props: {},
};
</script>

<style scoped lang="scss">
#logo {
  max-width: 200px;
}
</style>