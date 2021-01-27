<template>
  <router-link class="event-link" :to="{ name: 'EventDetails', params: { id: event.id } }">
    <div class="event-card">
      <span> @{{ event.time }} on {{ event.date }} </span>
      <h4>{{ event.title }}</h4>
    </div>
  </router-link>
</template>

<script>
export default {
  props: {
    event: {
      type: Object,
      required: true
    }
  }
}
</script>

<style scoped>
.event-card {
  padding: 1.2em;
  width: 20em;
  cursor: pointer;
  border: 1px solid #333;
  margin-bottom: 1em;
  transition: 0.2s ease;
}
.event-card:hover {
  transform: scale(1.1);
  transition: 0.2s ease;
}
.event-link{
  color:rgb(39, 107, 167);
  text-decoration: none;
}
</style>
