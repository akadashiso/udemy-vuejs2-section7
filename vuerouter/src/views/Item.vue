<template>
  <div>
    Item
    <router-link to="1">Item1</router-link>
    <router-link to="2">Item2</router-link>
    {{ $route.params.id }}
  </div>
</template>

<script>
export default {
  created() {
    console.log("created");
  },
  watch: {
    $route(to, from) {
      console.log(to);
      console.log(from);
    },
  },
};
</script>

<style>
</style>