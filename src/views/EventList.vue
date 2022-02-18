<template>
  <div class="events">
    <EventCard v-for="event in events" :key="event.id" :event="event" />
  </div>
</template>

<script>
// @ is an alias to /src
import EventCard from "@/components/EventCard.vue";

export default {
  name: "EventList",
  components: {
    EventCard,
  },
  data() {
    return {
      events: [
        {
          id: 592,
          category: "animal welfare",
          title: "Cat Adoption Day",
          description: "find your new feline friend at this event",
          location: "Meow town",
          date: "Jan 28 2022",
          time: "12pm",
          petAllowed: true,
          organizer: "Kat Laydee",
        },
        {
          id: 593,
          category: "animal welfare",
          title: "Cat Adoption Day",
          description: "find your new feline friend at this event",
          location: "Meow town",
          date: "Jan 28 2022",
          time: "12pm",
          petAllowed: true,
          organizer: "Kat Laydee",
        },
        {
          id: 594,
          category: "animal welfare",
          title: "Cat Adoption Day",
          description: "find your new feline friend at this event",
          location: "Meow town",
          date: "Jan 28 2022",
          time: "12pm",
          petAllowed: true,
          organizer: "Kat Laydee",
        },
      ],
    };
  },
};
</script>

<style scoped>
.events {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
