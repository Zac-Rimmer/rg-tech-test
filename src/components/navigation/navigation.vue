<template>
  <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link> |
      <router-link to="/regatta-group">Regatta Group</router-link>
    </div>
</template>

<script>
export default {
  name: "Navigation",
  props: {},
};
</script>
<style scoped lang="scss">
#nav {
  a {
      padding: 0 10px;
  }
}
</style>

