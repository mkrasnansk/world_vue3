<template>
  <div>
    <h1>Ooops!</h1>
    <h3>
      Network problems, please take a breath and
      <a href="#" @click="$router.go(-1)">Click here</a>
      <!-- naviguje na predoslu stranku -->
      to try again.
    </h3>
  </div>
</template>

<script>
export default {}
</script>

<style></style>
