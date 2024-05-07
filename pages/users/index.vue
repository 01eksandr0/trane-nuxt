<template>
  <div>
    <h2>Users</h2>
    <ul>
      <li v-for="user in users" :key="user.id">
        <a @click.prevent="$router.push('/users/' + user.id)">
          {{ user.name }}</a
        >
      </li>
    </ul>
  </div>
</template>

<script>
import { mapGetters } from "vuex";

export default {
  async fetch({ store }) {
    if (store.getters["users/users"].length === 0) {
      await store.dispatch("users/fetch");
    }
  },
  computed: {
    ...mapGetters("users", ["users"]),
  },
};
</script>

<style lang="css" scoped>
/* Add your styles here */
</style>
