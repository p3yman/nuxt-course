<template>
  <div>
    <div v-for="(title, slug) in posts">
      <h1><nuxt-link :to="`/blog/${slug}`">{{ title }}</nuxt-link></h1>
    </div>
  </div>
</template>

<script>
    export default {
        name: "index",

      data(){
          return {
            posts: {
              hello: 'Hello world',
              diary: 'Diary',
              'last-trip': 'Last trip',
            }
          }
      }
    }
</script>

<style scoped>

</style>
