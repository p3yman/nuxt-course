<template>
  <div>
    Blog single post
    {{ $route.params.slug }}
  </div>
</template>

<script>
  export default {
    name: "index",

    data(){
      return {
        post: null,
      }
    },
  }
</script>

<style scoped>

</style>
