<template>
  <header class="d-flex justify-content-between">
    <img src="../../assets/images/Regatta-Group-Logo.png" alt="Regatta Group" id="logo" />
    <div id="nav" class="col d-flex align-items-center justify-content-center">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>
  </header>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {},
};
</script>

<style scoped lang="scss">
#logo {
  max-width: 200px;
}

#nav {
    a {
        padding: 0 10px;
    }
}
</style>
