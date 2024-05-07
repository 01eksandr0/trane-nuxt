<template>
  <div>
    <NavBar />
    <main><nuxt /></main>
  </div>
</template>

<script>
import NavBar from "../components/NavBar.vue";
export default {
  comments: { NavBar },
};
</script>

<style lang="css">
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
</style>
