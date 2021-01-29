<template>
  <p>Register</p>
  <button @click="register">Register Me</button>
</template>

<script>
export default {
  props: ['event'],
  methods: {
    register() {
      //call API
      //If registered then redirect to event details

      // MOZNOSTI POUZITIA
      //       // Directly to the path with a single string
      // this.$router.push('/about')

      // // Directly to the path with an object
      // this.$router.push({ path: '/about' })

      // // Directly to the named path
      // this.$router.push({ name: 'About' })

      // // With a dynamic segment as I showed above
      // this.$router.push({ name: 'EventDetails', params: { id: 3 } })

      // // With a query ... resulting in /?page=2 in our example app
      // this.$router.push({ name: 'EventList', query: { page: 2 } })
      this.$router.push({
        name: 'EventDetails'
      })
    }
  }
}
</script>
