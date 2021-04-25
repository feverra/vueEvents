<template>
  <div class="events">
    <h1>Events For Good</h1>
    <EventCard
      v-for="event in events"
      :key="event.id"
      :event="event"
    ></EventCard>
  </div>
</template>

<script>
import EventCard from "@/components/EventCard.vue";
import axios from "axios";
export default {
  name: "Home",
  components: {
    // HelloWorld,
    // Product,
    EventCard,
  },
  data() {
    return {
      events: null,
    };
  },
  methods: {
    click() {},
  },
  created() {
    axios.get("http://localhost:8080/db.json").then((response) => {
      this.events = response.data.events;
    });
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