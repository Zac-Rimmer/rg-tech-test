<template>
  <header class="d-flex justify-content-between">
    <img src="../../assets/images/Regatta-Group-Logo.png" alt="Regatta Group" id="logo" />
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link> |
      <router-link to="/regatta-group">Regatta Group</router-link>
    </div>
</template>

<script>
export default {
  name: "Header",
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
