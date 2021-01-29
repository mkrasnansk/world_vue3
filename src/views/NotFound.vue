<template>
  <h1>Ooops!</h1>
  <h3>The {{ resource }} is not found!</h3>
  <router-link :to="{ name: 'EventList' }">Back to the home page</router-link>
</template>
<script>
export default {
  props: {
    resource: {
      type: String,
      require: true,
      default: 'page'
    }
  }
}
</script>
