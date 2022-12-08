<template>
  <div>
    <h1>User Slug Detail</h1>
    <p>id = ({{ id }})</p>
    <nuxt-link to="./">Back</nuxt-link>
  </div>
</template>

<script>
export default {
  validate({ params }){
    return params.slug === '1' || params.slug === '2'
  },
  data() {
    return {
      id: this.$route.params.slug,
    }
  },
  
}
</script>

<style></style>
