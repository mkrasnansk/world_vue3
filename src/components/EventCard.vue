<template>
  <div class="event-card">
    <span> @ {{event.time}} on {{event.date}} </span>
    <h4>{{event.title}} </h4>
  </div>
</template>

<script>
export default {
  name: "EventCard",
  props: {
    event: Object
  },
};
</script>

<style scoped>
.event-card{
  padding: 1.2em;
  width: 20em;
  cursor: pointer;
  border: 1px solid #333;
  margin-bottom: 1em;
  transition: .2s ease;

}
.event-card:hover{
  transform: scale(1.1);
  transition: .2s ease;
}
</style>
