<template>
  <div>
    <h2>User by Id</h2>
    <h4>ID: {{$route.params.id}}</h4>
  </div>
</template>

<script>
export default {
  validate(data) {
    return /^\d+$/.test(data.params.id);
  },
  layout: "users"
};
</script>

<style>
</style>
