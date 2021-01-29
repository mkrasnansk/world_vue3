<template>
  <div class="about">
    <h1>A site for events to better the world.</h1>
    <h1>You are on page {{}} </h1>
    <div v-if="showExtra">Page About</div>
  </div>
</template>
<script>
export default {
  props: route => {
    return { showExtra: route.query.e }
  }
}
</script>
