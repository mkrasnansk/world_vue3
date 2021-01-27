<template>
  <h1>Events For Good</h1>

  <div class="events">
    <EventCard v-for="event in events" :key="event.id" :event="event" />
  </div>
</template>

<script>
// @ is an alias to /src
import EventCard from "@/components/EventCard.vue";

export default {
  name: "Home",
  components: {
    EventCard
  },
  data() {
    return {
      events: [{
        id: 1,
        category: 'animal welfare',
        title: 'Cat Adoption Day',
        description: 'Find your new feline friend at this event,',
        location: 'New York',
        date: 'January 28, 2021',
        time: '12:00',
        petsAllowed: true,
        organizer: 'Michal Krasnansky'
      },
      {
         id: 2,
        category: 'animal welfare',
        title: 'Cat Adoption Day',
        description: 'Find your new feline friend at this event,',
        location: 'New York',
        date: 'January 28, 2021',
        time: '12:00',
        petsAllowed: true,
        organizer: 'Michal Krasnansky'
      }
      
      ]
    }
  },
};
</script>

<style scoped>
.events{
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
