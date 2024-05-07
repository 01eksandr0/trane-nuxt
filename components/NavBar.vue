<template>
  <div class="navbar">
    <ul class="list">
      <li>
        <nuxt-link exact no-prefetch active-class="active" to="/"
          >Home</nuxt-link
        >
      </li>
      <li>
        <nuxt-link no-prefetch active-class="active" to="/about"
          >About</nuxt-link
        >
      </li>
      <li>
        <nuxt-link no-prefetch active-class="active" to="/users"
          >Users</nuxt-link
        >
      </li>
      <li>
        <nuxt-link no-prefetch active-class="active" to="/login"
          >Login</nuxt-link
        >
      </li>
    </ul>
  </div>
</template>

<script>
export default {};
</script>

<style lang="css" scoped>
.navbar {
  height: 50px;
  width: 100%;
  background-color: aqua;
  display: flex;
  align-items: center;
  justify-content: center;
}
.list {
  display: flex;
  align-items: center;
  gap: 20px;
}
.active {
  color: brown;
}
</style>
