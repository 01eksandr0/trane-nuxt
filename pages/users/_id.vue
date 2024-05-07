<template>
  <div>
    <h1>User {{ $route.params.id }}</h1>
  </div>
</template>

<script>
export default {
  validate({ params }) {
    return true;
  },
};
</script>

<style lang="scss" scoped></style>
